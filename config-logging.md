# config-logging

## console
コンソールログの出力設定。

### sinkType
`Sync`,`ASync`がある。ロギングを同期的に行うか非同期的に行うかということだと思う。非同期だとクラッシュしたときなどに一部ログが欠ける場合が発生するはず。

### level
出力の粒度設定。

`Trace`,`Debug`,`Info`,`Warning`,`Error`,`Fatal`（左から右に行く順に出力が荒くなる）に加えて、`Max (Fatalのエイリアス)`と`Min (Traceのエイリアス)`がある。頭文字が大文字であることに注意。

### colorMode
出力の装飾設定

| mode     | description    |
| -------- | -------------- |
| Ansi     | Ansi code      |
| AnsiBold | bold Ansi code |
| None     | No coloring    |

## console.component.levels

> \# e.g. to log more verbose messages about the 'net' component, uncomment  
> \# net = Debug

部分的により詳細なログを出力させたいときに指定が出来る。上記の場合、`net`を

```
2019-02-26 07:03:11.507525 0x00007fa700fb4a80: <info> (plugins::PluginModule.cpp@79) loading plugin from ./libextension.eventsource.so
```

上記の`(plugins::PluginModule.cpp@79)`の部分( ::catapult::utils::ExtractDirectoryName(\_\_FILE\_\_)により出力されるのだと思う )がタグになり、これに反応してより詳細なログを出力させたければ、

> plugins = Debug

と書けば良い。

## file
ファイルに出力されるログの設定。

### sinkType
consoleの`synkType`参照

### level
consoleの`level`参照

### directory
ログファイルが出力されるディレクトリ

ディレクトリ名のみ又は相対パスによる指定をした場合は、カレントディレクトリからのパスでディレクトリが生成される。絶対パスによる指定も可能。

### filePattern
ログファイルの命名規則。

`catapult_server%4N.log`であれば、`catapult_server0000.log`のようなログファイルが生成され、`catapult_server%3N.log`であれば、`catapult_server000.log`のようなログファイルが生成される。

### rotationSize
ログファイル一つ分の最大容量

### maxTotalSize
ログファイル群全体での最大容量

### minFreeSpace
ログファイルを作成するための最小空きディスク容量。

## file.component.levels
consoleの`component.levels`参照。
