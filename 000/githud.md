
git add .

git commit -m "0909"

git push origin master 


#打开Git命令页面，执行git命令脚本：修改设置，解除ssl验证
问题：OpenSSL SSL_read: Connection was reset, errno 10054

git config --global http.sslVerify "false"


#在push远程服务器的时候发现出现此错误；原因是没有同步远程的master
 ! [rejected]        master -> master (fetch first)
git pull origin master

用git stash保存当前存储库，然后再进行所需的提交(将上游存储库中的更改与git stash pop合并后)