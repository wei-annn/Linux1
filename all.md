# Linux 課堂筆記
-----------------------

"#"最高權限管理者

"$"一般使用者

w 列出目前登入者帳號資訊

bash 提供命令輸入，行程控制，快速完成指令，顯示資訊顏色

<img width="88" alt="image" src="https://user-images.githubusercontent.com/81812410/173366845-5e83b92a-27a5-4606-910d-5193149ac487.png">

echo 顯示在螢幕

cat  把檔案內容顯示

curl 文字版的瀏覽器 測試網站OK嗎

su   系統管理員權限

vim 編寫檔案> a>寫字 esc>結束寫字> : > wq跳出

------------------------
如何一鍵把檔案內容清掉?

用:  (空白) > XX.sh

大於的意思:把前面丟到後面，因為前面是空的所以就清掉了

<img width="225" alt="image" src="https://user-images.githubusercontent.com/81812410/173338614-ba32fa68-53b7-4770-95d6-98da2c65776a.png">



-------------------------
uname -r 查版本

"快照"儲存虛擬機進度

虛擬機備份不建議直接複製貼上，建議用"匯入""匯出"

gedit XX.sh &  <&表示在背景執行，使可以繼續編輯

在Linux裡面，副檔名不代表任何意思，只是給人看，要看權限的指令: ls -l

-rw-rw-r-- 第一個"-"指的是檔案，如果是"d"是目錄，後面三個一組分別代表: 擁有者權限/擁有者群組權限/其他人權限

r:可讀

w:可寫

x:可執行

<img width="143" alt="image" src="https://user-images.githubusercontent.com/81812410/173349834-bc6fc93b-043e-455f-b81a-2d9a36667adf.png">

------------------------
.  : 當前目錄

..  : 上一層目錄

<img width="163" alt="image" src="https://user-images.githubusercontent.com/81812410/173350100-9057342c-d339-4cdc-8e04-041b3c21257b.png">

yum install httpd 安裝網頁伺服器

systemctl stop firewalld 關閉防火牆

<img width="199" alt="image" src="https://user-images.githubusercontent.com/81812410/173337893-ebabe070-865f-4f81-a0bc-fb24cfff58ea.png">


sudo -l 看使用者有沒有切換成超級使用者的權力和他可以執行甚麼超級使用者的指令

w : write

wq : write and quit

q : quit

q! : quit and give up modified things

!! : 上一個執行的指令(不用重新寫一長串指令)

<img width="188" alt="image" src="https://user-images.githubusercontent.com/81812410/173366094-33998afa-2e64-4a9d-bf2e-10fedc43a2fe.png">


chmod +x XX.sh :增加"執行"權限

-------------------------

看IP位址

windows : ipconfig

linus : ifconfig

-------------------------
馬上關機

halt -p

poweroff

shutdown -h now

取消關機 : shutdown -c

十分鐘後關機 : shutdown -h 10

立即重新啟動 : shutdown -r now

------------------------
! + 數字 : 執行 往上尋找

<img width="209" alt="image" src="https://user-images.githubusercontent.com/81812410/173340655-11b09a88-3518-45d5-b7e6-bdfdf9b23b56.png">

ctrl + a : 最前面，ctrl + e : 最後面

<img width="220" alt="image" src="https://user-images.githubusercontent.com/81812410/173341080-c59aaae4-88c6-4cac-8c81-9fd962e6ac5a.png">

whoami 顯示現在使用者

passwd 更變密碼

<img width="211" alt="image" src="https://user-images.githubusercontent.com/81812410/173349282-fba6509f-d5e7-4df5-b16a-805619459b79.png">

複製檔案 cp(copy)、移動檔案mv(move) 、刪除檔案 rm(remove)、刪檔不要詢問 : rm -f

<img width="298" alt="image" src="https://user-images.githubusercontent.com/81812410/173350477-635b12f4-ad3a-4d0a-bb07-0d388a37a1e5.png">
<img width="221" alt="image" src="https://user-images.githubusercontent.com/81812410/173350657-af88dc2a-9078-4cad-a3f5-fb071e68c66d.png">

相對路徑 cd etc 、cd httpd

絕對路徑 cd /etc/httpd/conf (直接指定要去的完整路徑名稱)

<img width="175" alt="image" src="https://user-images.githubusercontent.com/81812410/173353954-ce6e1445-ea68-4260-b62d-50cdc428e126.png">

新增檔案touch、觀看檔案cat、mkdir 建立資料夾(目錄)

<img width="302" alt="image" src="https://user-images.githubusercontent.com/81812410/173355758-8eb4efaa-b17c-45ae-8108-c4dbe6ab85ed.png">
<img width="292" alt="image" src="https://user-images.githubusercontent.com/81812410/173355801-179ad4ff-1217-4400-b8c2-f52acec064d7.png">



export PATH = $PATH (只在當前視窗有用)

source.bashrc : 生效 、 .bashrc : 隱藏檔

<img width="381" alt="image" src="https://user-images.githubusercontent.com/81812410/173358134-a9ec2179-57aa-4f7c-a94c-d386a3825d50.png">

<img width="357" alt="image" src="https://user-images.githubusercontent.com/81812410/173358246-efecaf6a-f529-49de-80c1-620e1634a9c8.png">

<img width="471" alt="image" src="https://user-images.githubusercontent.com/81812410/173358351-e478fefd-4fb4-439a-87b0-705bbca1ea93.png">

ls /tem : 動作、1>/dev/null 2>&1 : 指令

<img width="311" alt="image" src="https://user-images.githubusercontent.com/81812410/173361205-70134399-d483-4b78-b993-38bb2af67e86.png">
<img width="323" alt="image" src="https://user-images.githubusercontent.com/81812410/173361289-a2d14c74-fba0-4b8e-a138-0fd2dd5814b8.png">
<img width="184" alt="image" src="https://user-images.githubusercontent.com/81812410/173363867-6f9156fe-a70f-4d40-bac9-da8677d9d0d0.png">

寫完要加權限

echo & 可以看先前的指令是否成功，"0"為成功，其他的錯

腳本程式:

<img width="206" alt="image" src="https://user-images.githubusercontent.com/81812410/173364916-ad8b8f08-47f2-4ca1-8abe-7cdda1c730e2.png">
<img width="196" alt="image" src="https://user-images.githubusercontent.com/81812410/173364977-e2293359-2380-4955-b9b7-92696acab2c6.png">
<img width="198" alt="image" src="https://user-images.githubusercontent.com/81812410/173365076-5907cc17-dd21-4ed9-adec-23495f701743.png">

-i 不分大小寫

su vs su - :

<img width="205" alt="image" src="https://user-images.githubusercontent.com/81812410/173368642-269a2df7-3674-414a-b8f3-c0114e9e8a6a.png">

su 保有原來使用者的系統環境變量

su - root的系統環境變量

