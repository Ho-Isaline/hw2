# Linux

> 1.   一種作業系統
> 2.   類似於unit，但不是unit!!
> 3.   較不耗資源，
> 4.   常用來處理巨量資料
> 5.  雲端部署時常使用
> 6.  可移植性<br>

    ex: Ubunto(常用)

---
### 目錄指令 : 
- /     根目錄<br>
- /usr  使用者的應用程式和檔案都放在此(*類似與windows下的program files目錄*)<br>
- /tmp  供全部使用者暫時放置檔案的位置<br>
- /var  變動的資料或暫存檔(*log file*), 都會放置在此<br>
- /root 系統管理員(*超級許可權者的使用者主目錄*)<br>
- /bin  存放經常使用的命令<br>
- /boot 系統啟動時必須讀取的檔案<br>
- /home 存放普通使用者的家目錄(*每個使用者都有自己的家目錄*)<br>
---
### 兩種路徑
*   絕對路徑: 由根目錄 / 寫起<br>
        cd(移動目錄位置)/下層資料夾/資料
        
        ex: cd /test2/hello
        
*   相對路徑: 相對於目前工作目錄的路徑
        cd(移動目錄位置)/上層資料夾/上層(跟目錄)/下層資料夾/資料
        
        ex: cd ../../../test2/hello

#### 路徑相關符號指令
    .：  此層目錄
    ..： 上一層目錄
    -：  前一個工作目錄
    ~：  目前使用者身分所在的家目錄

### Linux指令
- cd        變換目錄
- ls        顯示目錄下的所有檔案
- pwd       顯示目前目錄的所在位置
- cat       查看檔案內容
- vi        編輯檔案
- mkdir     建立一個新目錄
- mkdir -p  同時建立多個目錄
- rmdir     刪除一個裡面是空的空目錄
- rm        刪除檔案
- rm -r     強制刪除
- mv        移動，重新命名
#### 特殊指令
>   - **更改使用者權限**   
>   
>       **chmod**
>   
>       - 身分分類
>           <pre><code>  u -> 檔案擁有者
>           g -> 與該檔案的  擁有者同一個群體者
>           o -> 其他以外的人
>           a -> 三者皆是</code></pre>
>
>       - 設定許可權
>            <pre><code>   +：增加許可權
>            -：取消許可權
>            =：唯一設定許可權</code></pre>
>
>       - 權限項目
>            <pre><code>   r：可讀取
>            w：可寫入
>            x：可執行</code></pre>


>   - **壓縮與解壓縮**    
>
>       **gzip**<br>
>       - 壓縮：
>           <pre><code>  gzip FileName</code></pre>
>           
>       - 解壓縮：
>           <pre><code>  gunzip FileName.gz
>           gzip -d FileName.gz</code></pre>
>
>       **xz**
>       - 壓縮：
>           <pre><code>  xz -z FileName</code></pre>
>           
>       - 解壓縮：
>           <pre><code>  xz -d FileName.xz</code></pre>
>
>       **tar.gz**<br>
>       - 壓縮：
>           <pre><code>  tar -zcvf FileName.tar.gz DirName</code></pre>
>           
>       - 解壓縮：
>           <pre><code>  tar -zxvf FileName.tar.gz9</code></pre>

>   - **檔案內容查閱**<br>
>   
>       **cat**<br>
>       
>       <pre><code>  -n: 由1開始對所有輸出的行數編號
>       >: 將多個文件覆蓋到目標文件中
>       >>: 將多個文件追加到目標文件中，不覆蓋</code></pre>
>
>       **head**    取出前面幾行(*預設10行*)<br>
>       <pre><code>  -n：後面接數字，代表幾行的意思
>       -n +20：只想列出20行以前的資料</code></pre>
>       
>       **tail**    取出後面幾行(*預設10行*)<br>
>       <pre><code>  -n：後面接數字，代表幾行的意思
>       -n +20：只想列出20行以後的資料</code></pre>
---
### nano
