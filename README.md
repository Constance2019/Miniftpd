# Miniftpd
项目简介：提供文件存储和访问服务，实现信息共享
开发环境：CentOS、 C/C++、 Gcc、 Makefile、 Editplus、 LeapFtp客户端, Git
主要技术：socket、IO复用、IPC、HashTable
项目特点：
1、实现Ftp内部标准命令USER、PASS 、PORT、 PASV、 LIST、 STOR、 RETR 、RNFR、 RNTO、MKD、 RMD…..
2、实现配置文件的解析
3、实现用户鉴权登录功能
4、实现FTP两种模式<主动模式port, 被动模式pasv>的数据连接建立
5、实现文件的上传、续传、下载、续载功能，上传下载限速功能
6、实现系统的空闲断开<数据连接断开，控制连接断开>，系统的连接数限制<客户连接数限制，每IP连接数限制>
项目难点:    nobody进程协助ftp进程绑定20端口
            数据连接建立过程中的主动模式以及被动模式的理解
          	每IP连接数限制的实现过程，为统计每IP的连接数，需要借助两个Hash表完成映射

