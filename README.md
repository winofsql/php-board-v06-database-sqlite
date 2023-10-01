# php-board-v06-database-sqlite

- PHP 側の入力チェックとエラーメッセージ
- データーベース仕様に変更
- 表示データの脆弱性対応

```sql
CREATE TABLE IF NOT EXISTS `board` (
  `row_no` bigint(20) NOT NULL PRIMARY KEY AUTOINCREMENT,
  `body` varchar(1000) DEFAULT NULL,
  `subject` varchar(200) DEFAULT NULL,
  `from` varchar(20) DEFAULT NULL,
  `pdate` datetime DEFAULT NULL,
  `cdate` datetime DEFAULT NULL,
  `dflg` varchar(1) DEFAULT NULL,
  `image` varchar(100) DEFAULT NULL
)
```
