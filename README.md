1、先在服务器上安装好 ss-panel ,注意要将 Shadowsocks-manyuser 的数据库一起导入，本程序使用相同的数据库，兼容。
2、然后 搭建好 java 运行环境，并将 https://github.com/shadowsocks/shadowsocks-libev 按照步骤安装好。
3、在数据库上添加一个远程用户。
4、运行

screen -dmS shadowsocksshell java -jar shadowsocksshell.jar <数据库地址> <数据库名称> <数据库用户名> <数据库密码> <服务器公网IP>

5、可添加上面一行命令到 /etc/rc.local 实现开机启动。
