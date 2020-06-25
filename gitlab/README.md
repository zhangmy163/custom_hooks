是根据接收到的三个参数，再结合git的相关命令，来实现控制提交等。
   oldrev=$(git rev-parse $1)
   newrev=$(git rev-parse $2)
   refname="$3"


文件放在`/var/opt/gitlab/git-data/repositories/[devgit]/[demo.git]/custom_hooks/pre-receive`

赋权`sudo chown -R git:git xxxx/pre-receive`

赋权`sudo chmod +x xxxx/pre-receive`

限制gitlab提交注释和分支名称
