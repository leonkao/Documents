# Xmlportletfactory使用說明

## Xmlportletfactory安裝說明

	-http://www.xmlportletfactory.org/ 
	-https://sourceforge.net/projects/xmlportlet/files/For%20Liferay%206.0.x/
	-http://ant.apache.org/

### 網址A為Xmlportletfactory的官方網站
### 網址B為Xmlportletfactory的下載網站,在此選擇的版本為“XMLPortletFactory_6.x-v3.0.zip”
### 網址C為Xmlportletfactory所需要的軟體,主要是在windows os上需要下載該軟體,在此選擇的版本為Apache Ant 1.9.7

---

## 1.在下載完XMLPortletFactory的檔案解壓縮後會有這些檔案如圖

#![](XMLPortletFactory/image/XMLPortletFactory001.png)

## 2.將整個資料夾移動放置自己設定liferay的sdk資料夾裡面如圖

#![](XMLPortletFactory/image/XMLPortletFactory002.png)

## 3.下載Apache-ant 並解壓縮到自己設定的資料夾內

#![](XMLPortletFactory/image/XMLPortletFactory003.png)

## 4.由於需要使用一些command line指令，而在windows上直接輸入是不會有任何回應的，所以需要設定一些環境變數，如ant.

## 5.所以將需要的檔案放置好個資料夾後開始設定環境變數
## 6.點選我的電腦右鍵內容-->進階系統設定-->系統內容

#![](XMLPortletFactory/image/XMLPortletFactory004.png)

## 7.點選下方環境變數

#![](XMLPortletFactory/image/XMLPortletFactory005.png)

## 8.在此新增一個環境變數為，變數名稱： ANT_HOME  變數值：C:\JAVA\apache-ant-1.9.7 (你所放置之apache-ant的資料夾)

## 9.接下來在環境變數裡編輯Path變數的值，在值的後面增加  %ANT_HOME%\bin;%JAVA_HOME%\bin;%JAVA_HOME%\jre\bin;

#![](XMLPortletFactory/image/XMLPortletFactory006.png)

## 10.開啟命令提示字元輸入自己設定的Xmlportletfactory資料夾內

#![](XMLPortletFactory/image/XMLPortletFactory007.png)

## 11.開一個新的Xmlportletfactory檔案 
	-create.bat max “max”   ==>	create.bat (檔名) “資料夾名稱”

#![](XMLPortletFactory/image/XMLPortletFactory008.png)

## 12.Build successful後會在xmlportletfactory裡面出現一個max-xmlportletfactory的資料夾然後進入該資料夾再輸入ant
## 13.Build successful後表示成功

#![](XMLPortletFactory/image/XMLPortletFactory009.png)

## 14.進入eclipse -->import一個Liferay Projects From Plugins SDK

#![](XMLPortletFactory/image/XMLPortletFactory010.png)

## 15.選擇max-porlet(C:\JAVA\liferay-plugins-sdk-6.2\portlets\max-portlet)

#![](XMLPortletFactory/image/XMLPortletFactory011.png)

## 16.進入liferay網頁後再增加applications部分下便可以看到max這個portlet的部分出現在上面

#![](XMLPortletFactory/image/XMLPortletFactory012.png)

## 17.要編輯他的相關檔案則是在自己設定的資料夾(本文的為下列位址)
C:\JAVA\liferay-plugins-sdk-6.2\XMLPortletFactory\max-xmlportletfactory
裡面的max.xml檔案進行編譯即可。

