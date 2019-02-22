# catapult.tools.health

DiagnosticCounterから取得でき、`catapult.tools.health`によって取得できるステータスの意味をまとめる。

| name          | full name                                 | description                                                    |
| ------------- | ----------------------------------------- | -------------------------------------------------------------- |
| ACNTST C      | AccountStateCache                         | キャッシュ内に存在するAccountの数                              |
| ACNTST C HVA  | AccountStateCache highValueAddresses      | ハーベスティング可能Account数                                  |
| ACTIVE PINGS  | Active Pings                              | 現在ハンドシェイク中のコネクション数？                         |
| B WRITERS     | Broadcast Writer ?                        | APIネットワークへブロードキャストするパケットライターの数？    |
| BLK ELEM ACT  | Block Elements Active                     |                                                                |
| BLK ELEM TOT  | Block Elements (Total?)                   | キャッシュに保存されているBlockElement総数                     |
| BLKDIF C      | BlockDifficulty Cache                     |                                                                |
| HASH C        | HashCache                                 | HashCacheはTxのhashを管理するキャッシュ？                      |
| HASHLOCK C    | HashLock Tx Cache                         |                                                                |
| MEM CUR RSS   | Memory Current ResidentSetSize?           |                                                                |
| MEM CUR VIRT  | Memory Current VirtualSetSize?            |                                                                |
| MEM MAX RSS   | Memory Max ResidentSetSize?               |                                                                |
| MEM SHR RSS   | Memory Share ResidentSetSize?             |                                                                |
| MOSAIC C      | Mosaic Cache                              | Mosaicの数                                                     |
| MULTISIG C    | Mutlisig Cache                            | MultisigAccountの数                                            |
| NS C          | NameSpace Cache                           | NameSpaceの数                                                  |
| NS C AS       | NameSpace Cache ActiveSize                | アクティブなNamespace数？                                      |
| NS C DS       | NameSpace Cache DeepSize                  |                                                                |
| PROPERTY C    | Property Cache                            | AccountProperties?                                             |
| RB COMMIT ALL | Rollback Elements Committed All           |                                                                |
| RB COMMIT RCT | Rollback Elements Committed Recent        |                                                                |
| RB IGNORE ALL | Rollback Elements Ignored All             |                                                                |
| RB IGNORE RCT | Rollback Elements Ignored Recent          |                                                                |
| READERS       | Readers                                   | ActiveなReaderの数(どこにも接続していなくても一つはアクティブ) |
| SECRETLOCK C  | SecretLock Cache                          |                                                                |
| SUCCESS PINGS | Success Pings                             | 成功したハンドシェイク数？                                     |
| TASKS         | Tasks                                     | 起動中のタスクの数                                             |
| TOT CONF TXES | Total Confirmed Transactions              | confirmしたTxの総数？                                          |
| TOTAL PINGS   | Total Pings                               | ハンドシェイク総数？                                           |
| TS NODE AGE   | TimeSynchronization Node Age              | 接続中のNodeAge(最高？)                                        |
| TS OFFSET ABS | TimeSynchronization Offset Direction      |                                                                |
| TS OFFSET DIR | TimeSynchronization Offset absoluteOffset |                                                                |
| TS TOTAL REQ  | TimeSynchronization Total Request         |                                                                |
| TX ELEM ACT   | Tx Element Actice                         |                                                                |
| TX ELEM TOT   | Tx Element Total                          |                                                                |
| UNLKED ACCTS  | Unlocked Accounts                         | そのノードで現在harvestingを行っているアカウント数             |
| UT CACHE      | Ut(Unconfirmed Tx) Cache                  |                                                                |
| WRITERS       | Writers                                   | ActiveなWriterの数(どこにも接続していなければ0)                |
