下載JDK 的安裝檔放在 docker-test資料夾裡，使用的版本是 jdk-8u152
以上的 Dockerfile 主要有用到的指令說明如下
FROM： 使用到的 Docker Image 名稱，今天使用 CentOS

### MAINTAINER： 用來說明，撰寫和維護這個 Dockerfile 的人是誰，也可以給 E-mail的資訊

### RUN： RUN 指令後面放 Linux 指令，用來執行安裝和設定這個 Image 需要的東西

### ADD： 把 Local 的檔案複製到 Image 裡，如果是 tar.gz 檔複製進去 Image 時會順便自動解壓縮。Dockerfile 另外還有一個複製檔案的指令 COPY 未來還會再介紹

### ENV： 用來設定環境變數

### CMD： 在指行 docker run 的指令時會直接呼叫開啟 Tomcat Service

需先下載 jdk-8u192-linux-x64.tar.gz 與 apache-tomcat-8.5.37.tar.gz 至此目錄
cmd 執行 docker build .
如有錯誤 sudo docker build .
