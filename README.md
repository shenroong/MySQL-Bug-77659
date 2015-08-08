# MySQL-Bug-77659

A bug fix for 
https://bugs.launchpad.net/percona-server/+bug/1469901?comments=all
and 
http://bugs.mysql.com/bug.php?id=77659

Basic idea is to check any other indexes use those columns. If this columns is used in other indexes, ord_part remains 1, otherwise ord_part becomes 0.