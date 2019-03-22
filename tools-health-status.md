# catapult.tools.health

DiagnosticCounterから取得でき、`catapult.tools.health`によって取得できるステータスの意味をまとめる。

| name          | full name                                 | description                                                                        |
| ------------- | ----------------------------------------- | ---------------------------------------------------------------------------------- |
| ACNTST C      | AccountStateCache                         | キャッシュ内に存在するAccountの数                                                  |
| ACNTST C HVA  | AccountStateCache highValueAddresses      | ハーベスティング可能Account数                                                      |
| ACTIVE PINGS  | Active Pings                              | 現在ハンドシェイク中のコネクション数？                                             |
| B WRITERS     | Broadcast Writer                          |                                                                                    |
| BLK ELEM ACT  | Block Elements Active                     |                                                                                    |
| BLK ELEM TOT  | Block Elements Total                      | Blockエレメント総数                                                                |
| BLKDIF C      | BlockDifficulty Cache                     |                                                                                    |
| HASH C        | HashCache                                 | HashCacheはTxのhashを管理するキャッシュ？                                          |
| HASHLOCK C    | HashLock Tx Cache                         |                                                                                    |
| MEM CUR RSS   | Memory Current ResidentSetSize            |                                                                                    |
| MEM CUR VIRT  | Memory Current VirtualSetSize             |                                                                                    |
| MEM MAX RSS   | Memory Max ResidentSetSize                |                                                                                    |
| MEM SHR RSS   | Memory Share ResidentSetSize              |                                                                                    |
| MOSAIC C      | Mosaic Cache                              | Mosaicの数                                                                         |
| MULTISIG C    | Mutlisig Cache                            | MultisigAccountの数                                                                |
| NS C          | NameSpace Cache                           | NameSpaceの数                                                                      |
| NS C AS       | NameSpace Cache ActiveSize                | アクティブなNamespace数？                                                          |
| NS C DS       | NameSpace Cache DeepSize                  |                                                                                    |
| PROPERTY C    | Property Cache                            | AccountProperties?                                                                 |
| RB COMMIT ALL | Rollback Elements Committed All           | ロールバックした回数                                                               |
| RB COMMIT RCT | Rollback Elements Committed Recent        | 最近ロールバックした回数(※"最近"は設定により異なる)                                |
| RB IGNORE ALL | Rollback Elements Ignored All             | ロールバック検証の末、ロールバックせずに無視した回数？                             |
| RB IGNORE RCT | Rollback Elements Ignored Recent          | 最近ロールバック検証の末、ロールバックせずに無視した回数？                         |
| READERS       | Readers                                   | ActiveなReaderの数(どこにも接続していなくても一つはアクティブ)                     |
| SECRETLOCK C  | SecretLock Cache                          |                                                                                    |
| SUCCESS PINGS | Success Pings                             | 成功したハンドシェイク数？                                                         |
| TASKS         | Tasks                                     | 起動中のタスクの数                                                                 |
| TOT CONF TXES | Total Confirmed Transactions              | confirmしたTxの総数                                                                |
| TOTAL PINGS   | Total Pings                               | ハンドシェイク総数？                                                               |
| TS NODE AGE   | TimeSynchronization Node Age              | 接続中のNodeAge(最高？)                                                            |
| TS OFFSET ABS | TimeSynchronization Offset absoluteOffset |                                                                                    |
| TS OFFSET DIR | TimeSynchronization Offset Direction      |                                                                                    |
| TS TOTAL REQ  | TimeSynchronization Total Request         |                                                                                    |
| TX ELEM ACT   | Tx Element Active                         |                                                                                    |
| TX ELEM TOT   | Tx Element Total                          | ノード立ち上げ間に処理したTxの総数（重複、検証失敗のものを含む全ての処理数）       |
| UNLKED ACCTS  | Unlocked Accounts                         | そのノードで現在harvestingを行っているアカウント数                                 |
| UT CACHE      | Ut(Unconfirmed Tx) Cache                  | キャッシュに存在する未承認Tx数（ブロックに格納されたUTはキャッシュから削除される） |
| WRITERS       | Writers                                   | ActiveなWriterの数(どこにも接続していなければ0)                                    |
