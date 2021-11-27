# Linux
> 
> 1.   一種作業系統
> 2.   類似於unit，但不是unit!!
> 3.   較不耗資源，
> 4.   常用來處理巨量資料
> 5.  雲端部署時常使用
> 6.  可移植性<br>


    ex: Ubunto(常用)

---
### 目錄指令 : 
- /：根目錄，所有檔案皆從根目錄開始，只有root使用者具該目錄的許可權<br>
- /root：該目錄為系統管理員，也稱作超級許可權者的使用者主目錄<br>
- /bin：存放著經常使用的命令<br>
- /boot：系統啟動時必須讀取的檔案, 包括系統核心<br>
- /home：存放普通使用者的家目錄，每個使用者都有自己的家目錄<br>
- /etc：放置與系統設定、管理相關的檔案<br>
- /usr：這是一個非常重要的目錄，使用者的應用程式和檔案都放在這個目錄下，類似與windows下的program files目錄<br>
- /media：可用來做為光碟、軟碟片、隨身碟與其他分割區的自動掛載點<br>
- /tmp：供全部使用者暫時放置檔案的目錄<br>
- /var：系統執行時, 內容經常變動的資料或暫存檔(log file), 都會放置在這個目錄裡<br>
---
### Linux指令
- cd        變換目錄
- pwd       顯示目前的目錄的所在位置
- ls        顯示目錄下的所有檔案
- touch     建立檔案
- cp        複製
- cat       查看檔案內容
- vi        編輯檔案
- mkdir     建立一個新目錄
- mkdir -p  同時建立多個目錄
- rmdir     刪除一個裡面是空的空目錄
- rm        刪除檔案
- rm -r     強制刪除
- mv        移動，重新命名
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
        
<p>This is a normal paragraph:</p>

<pre><code>This is a code block.
</code></pre>
Here is an example of AppleScript:

    tell application "Foo"
        beep
    end tell
<p>Here is an example of AppleScript:</p>

<pre><code>tell application "Foo"
    beep
end tell
</code></pre>

*文字*
**文字**
<table>
    <tr>
        <td>Foo</td>
    </tr>
</table>
