#### 基本的Linux操作命令

查询文件夹中文件的个数（不包含子文件夹）
>ls -l | grep "^-" | wc -l

注释：其中"^-"是一个正则化项，表示字符串的第一个字符。如果要查询子文件夹个数用 "^d"

查询文件夹中文件的个数（包含子文件夹）
>ls -lR | grep "^-"| wc -l

查看进程
>ps aux | grep nginx
