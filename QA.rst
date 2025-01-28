QA
==

2025-1-21
---------

我在github上建立了一個儲存庫，然後我要把我的程式push到github上的時候，卻遇到了問題，我告訴你我是如何解決的 
    > git remote add origin git@github.com:fc201127/Python.git
    > git branch -M main
    > git push -u origin main
    遇到了問題:
        remote: Support for password authentication was removed on August 13, 2021.
        remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls 
        for information on currently recommended modes of authentication.
        fatal: Authentication failed for 'https://github.com/A1234567890000000/Python.git/'
    如何解決???
    > cat ~/.ssh/id_rsa.pub
    你會看到:ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCatNCFx7DEhWaCzRQZJIc8p44gydZGMEKzFoisJ9+PaY/SXqOh7ba6oeoBNP3I6JW6Z8MSMUwTGmfk2BKOqszSTUURFW1IDoYeHc1tAw5xaU1XMvETonrLiR0irUnZcQY4ZTe/SdQVD+MNqAND5uFOHp+3cihUlyhrkIsDcqUZ7k5jMZRL4a3K5AMuhtYmjuPgmCKfO3CsNYYud0twkLJEyNGjDHYv7FU3eQOXm7KFDEnymdCDPRWFongiV+RTdl92WnZ/y+UudvIJl/pTcJcVZf8WD8uoy2AC9iRFl0oFQCVQnDTJkJ3QlIfh+dVZkfHhD/oZSLDpp1o84gVwvBTadB2ol6qTrZC8CiKgVNuBMGHtH+eDW62IRM2A4sttZhW9plnOsyoGOz4hCWAMGGe2Jsrz4lFRHirdwwWIczB7MENAiRrFHoOyRcy0AMAJ49MQGtTGXERJ4JuqlJGxk72JkttGTKKOiMQYd7QhYtxDtAMloCqYuRG9NV+T6JUUsqU= ben@tp07
然後:
    登入您的 GitHub 帳戶。
    點擊右上角的個人頭像，選擇「Settings」進入設定頁面。
    在左側選單中，點擊「SSH and GPG keys」。
    點擊「New SSH key」，將 id_rsa.pub 檔案的內容複製並貼上到「Key」欄位中。
    點擊「Add SSH key」以完成添加。
    > git remote set-url origin git@github.com:your_username/your_repository.git
    > git push -u origin main
    你應該會看到:
        Enumerating objects: 48, done.
        Counting objects: 100% (48/48), done.
        Delta compression using up to 4 threads
        Compressing objects: 100% (36/36), done.
        Writing objects: 100% (48/48), 7.46 KiB | 1.49 MiB/s, done.
        Total 48 (delta 14), reused 0 (delta 0), pack-reused 0
        remote: Resolving deltas: 100% (14/14), done.
        To github.com:fc201127/Python.git
        [new branch]      main -> main
        branch 'main' set up to track 'origin/main'.
        表示你成功上傳
