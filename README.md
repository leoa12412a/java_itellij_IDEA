# java_itellij_IDEA

### 在 Windows 系統下安裝 itellij IDEA 

進入官網(https://www.jetbrains.com/idea/)下載 itellij IDEA 的可執行文件

有分Ultimate(旗艦版) 和 Community(社區版)

旗艦版是收費的，而社區版是免費的，旗艦版的筆社區版的功能更全面，安裝的項目基本上都是下一步就可以了。

安裝完後第一次開啟程式會長這樣，按下Create new project來建立一個新的專案

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/1.PNG)</br></br>

建立好之後，我們需要使用右上角的New 按鈕幫我們的專案裝上JDK(java SDK)

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/2.PNG)</br></br>

而JDK可到https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html下載

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/3.PNG)</br></br>

設定完JDK後，IDEA會詢問是否需要建立樣板 ， Command Line App會建立一個包含主函式(main)的樣板，而Java Hello World當然就是執行hello world

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/4.PNG)</br></br>

最後只需要輸入專案名稱就可以了

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/5.PNG)</br></br>

建立好專案後，可以看到左手邊就是我們的專案資料夾，而專案下的src就是source code的縮寫，這時候我們在src右鍵建立一個java class

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/6.png)</br></br>

建立java class的時候如果輸入 myjava.helloworld ，意思就是myjava這包(package)下面的helloworld.java，所以如果想在同一個package建立的時候需要特別留意

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/7.PNG)</br></br>

建立好之後會看到頁面最上方已經有寫上package，且基本的public class也建立好了，這時候我們需要建立一個主函式(main)
輸入psvm是建立主函式的快捷鍵，也是public static void main的縮寫

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/8.png)</br></br>

再來就是建立輸出文字，一樣這個也有快捷鍵，sout，是System.out.println()的縮寫

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/9.png)</br></br>

再來執行的話，點選上方Run->Run '專案名稱'，如果有package的話需要修改Run->Edit Configrations
->Application->專案名稱->Main class->'package名稱.專案名稱'

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/10.png)</br></br>

執行後就可以在下方欄位看到輸出結果，下方還有一個terminal按鈕，跟本機終端是一樣的東西

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/11.PNG)</br></br>

### 使用終端機執行java檔案

java格式的檔案可以在終端機使用javac XXX.java把檔案變成java.class，在輸入java 檔案名稱，就可以執行了。

如果已經安裝JDK但是還是找不到javac指令的時候，到控制台->系統->進階系統設定>進階->環境變數->系統變數->Path(編輯)->瀏覽->/JDK/bin

![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/12.png)</br></br>

如果執行中文的時候發生亂碼錯誤，cmd：javac  -encoding utf-8  xx.java
也可以到 控制台->系統->進階系統設定>進階->環境變數->系統變數(新增)->
變數名稱 : JAVA_TOOL_OPTIONS
變數值 : -Dfile.encoding=UTF-8
這樣以後每次執行都會是UTF-8
![image](https://github.com/leoa12412a/java_itellij_IDEA/blob/master/13.PNG)</br></br>

