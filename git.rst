git
===

git是版本控管的工具，他可以讓你每一個版本都可以留下記錄，所以git的差別就是你一定要寫一些東西，不然他就commit不上去
git的命令大致上是以下:
    > git config --global user.name 你的姓名
    > git config --global user.email 你的電子郵件地址
    你下了這兩個命令會被存到~/.gitconfig裡面
    > vi gitdemo.txt
    gitdemo:
        Hello
    > git init
    > git add .(git add gitdemo.txt)
    > git commit -m "Initial commit"
    > vi gitdemo.txt
    gitdemo:
        Hello 123
    > git add .(git add gitdemo.txt)
    > git commit -m "Append 123"
    > git log
    你下了git log顯示的結果會是兩筆記錄，一筆是Inital commit 一筆是Append 123
    影片連結:https://www.youtube.com/watch?v=8f6k0_yG8TE&t=22s
             https://www.youtube.com/watch?v=KwHzjykRzMQ

