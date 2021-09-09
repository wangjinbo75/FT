
git add .

git commit -m "0909"

git push origin master 


#打开Git命令页面，执行git命令脚本：修改设置，解除ssl验证
问题：OpenSSL SSL_read: Connection was reset, errno 10054

git config --global http.sslVerify "false"
