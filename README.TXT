アプリケーション名        
  adhoc-wifi-tether

ソースのオリジナルのサイト
  https://code.google.com/p/android-wifi-tether/

アプリケーションの説明
  このアプリケーションは、android端末の無線LANインタフェースをAd-Hocモードに変更し、通信を可能にする。
  (android端末では、あらかじめroot取得を行う必要がある。root取得方法は使用するandroid機によって異なるので、調べてください）

テスト済みの環境
  motorola製 photon isw11m（android2.3.4/linux2.6.32.9-00138-g12ebd9ew21679@zkr30inxdroid19 #2)

TODOの項目
  +defaultではパケット受信処理は他端末からの接続要求があったときに起動する。これをアプリ開始時
  「常に受信待ち」に変更する
  +DHCPサーバは使用せず、固定IPアドレスを割り当てられるように変更する
  

--
Original README file of adhoc wifi teher describes following text.

WiFi Tether for Root Users
--------------------------

WiFi Tether for Root Users

*** Use this application at your own risk. It is possible that use of this program may violate your carrier's Terms of Use/Terms of Service. ***

This program enables wifi-tethering for "rooted" handsets.

Clients (your laptop for example) can connect via wifi and get access to the internet using the mobile connection (4G, 3G, 2G) of your phone.

Wifi-tethering creates a so called adhoc (peer-to-peer) network on most devices. 
Infrastructure-mode is supported for a large set of devices.

** PREREQUISITE **

1) Root
2) Netfilter-enabled kernel (most stock-kernel nowadays come with such a kernel).
