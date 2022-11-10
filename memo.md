### 接続スレッド数
```
show status like 'Threads_connected';
```
### プロセスリスト
```
show processlist;
```

```
mysql> show processlist;
+-----+------+------------------+---------------+---------+-------+-------------+---------------------------------+
| Id  | User | Host             | db            | Command | Time  | State       | Info                            |
+-----+------+------------------+---------------+---------+-------+-------------+---------------------------------+
|   4 | root | 172.18.0.1:55100 | denshikeiyaku | Sleep   |   380 |             | NULL                            |
|   5 | root | 172.18.0.1:55104 | denshikeiyaku | Sleep   |   380 |             | NULL                            |
| 480 | root | 172.18.0.1:57020 | denshikeiyaku | Sleep   | 46553 |             | NULL                            |
| 481 | root | 172.18.0.1:57022 | denshikeiyaku | Sleep   |  2043 |             | NULL                            |
| 482 | root | 172.18.0.1:57024 | denshikeiyaku | Sleep   | 46727 |             | NULL                            |
| 623 | root | localhost        | NULL          | Query   |     0 | starting    | show processlist                |
| 629 | root | 172.18.0.8:43704 | denshikeiyaku | Query   |     0 | System lock | TRUNCATE `dkcabinet_upload_log` |
+-----+------+------------------+---------------+---------+-------+-------------+---------------------------------+

最終行がjest実行時のプロセス
```
