# [Git 新手上路 AMA](https://business.facebook.com/will.fans/videos/1806894692673000/) 實作練習腳本
# [Git 新手上路 AMA](https://gist.github.com/doggy8088/e39cfa2f28cd6da43fcf1689cee3f5ff?fbclid=IwY2xjawH9NVlleHRuA2FlbQIxMAABHeH1sYwR7OTF31Aw6Sj0dr0OcHfYNsg0G8HwIcjsHpSBUOm63HflRIc0KA_aem_WyRFBe7lxLGzmijdb3Qwjg) 原文連結

## 1. 安裝 Git 工具
dnf install git

## 2. 初始設定

每位 Git 新手上路都必須事先設定的兩行命令，設定你在版控時要顯示的 Name 與 Email 欄位。

  ```
  git config --global user.name 你的姓名
  git config --global user.email 你的電子郵件地址
  ```

## 3. 初始化儲存庫

  ```
  git init
  ```

## 4. 建立版本

  ```
  git add .
  git commit -m "Initial commit"
  ```

## 5. 查看版本紀錄

  ```
  git log
  ```

## 6. 建立分支

  建立分支

  ```
  git branch develop
  ```

  建立分支並切換至新分支

  ```
  git checkout -b develop
  ```

## 7. 切換分支

  顯示所有分支

  ```
  git branch
  ```

  切換分支

  ```
  git checkout develop
  ```

## 8. 建立標籤

  ```
  git tag v1.0
  ```

  ```
  git tag -a v1.0
  ```

## 9. 推送版本

  ```
  git remote add origin https://github.com/doggy8088/gitdemo.git
  git push -u origin master
  ```

  ```
  git push
  ```

## 10. 拉取版本

  ```
  git pull
  ```

## 相關連結

* [30 天精通 Git 版本控管](https://github.com/doggy8088/Learn-Git-in-30-days)
* [直播影片網址](https://business.facebook.com/will.fans/videos/1806894692673000/)
