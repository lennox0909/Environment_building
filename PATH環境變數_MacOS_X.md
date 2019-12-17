# PATH環境變數 Mac OS X

修改系統路徑($PATH)的方法：(來源為這裡)

方法是透過修改 .bash_profile 來達成
這個檔案會在使用者登入時執行
所以是針對使用者的，並不會影響其他帳號

1. 打開終端機
2. touch ~/.bash_profile; open ~/.bash_profile
3. 將路徑輸入在檔案裡
export PATH="/aaa/bb/bin:$PATH"
export PATH="/xxx/yyyy/bin:$PATH"
4. 存檔並關閉編輯器
5. source ~/.bash_profile 
這可以讓系統去執行 .bash_profile 使路徑馬上生效

這樣就完成了。現在可以檢查一下路徑
echo $PATH

=====================

列出環境變數
printenv

列出環境變數下的 Path
echo $PATH

打開 bash profile
vi ~/.bash_profile

新增路徑到 PATH
export PATH=$PATH:路徑名稱

存擋
:wq

執行 bash profile
source ~/.bash_profile
