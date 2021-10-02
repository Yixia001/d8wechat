"# d8wechat"
http://dev.d8wechat.local 
yxadmin


d8wechat
mysqldump  --default-character-set=utf8  --user=root --password=root --result-file=d8wechat0427.sql d8wechat

mysql -uroot -plogic123 -e "drop database if exists d8wechat"
mysql -uroot -plogic123 -e "create database if not exists d8wechat"
mysql -uroot -plogic123 -e "source d8wechat0427.sql" d8wechat
pause

d7wechat
mysqldump  --default-character-set=utf8  --user=root --password=root --result-file=d7wechat0521.sql d7testdb

mysql -uroot -plogic123 -e "drop database if exists d7wechat"
mysql -uroot -plogic123 -e "create database if not exists d7wechat"
mysql -uroot -plogic123 -e "source d7wechat0521.sql" d7wechat
pause