[![BTO-logo](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/05/logo.png)](https://bit-trade-one.co.jp/)

BTIRSW リモート変わる君を使用する際に必要になる情報を掲載しています。  
下記項目リンクよりご覧になりたい情報にクリックすると該当部分へ移動します。  

### [リモート変わる君HPリンク](http://bit-trade-one.co.jp/btirsw)
### [開発情報(GitHub)](https://github.com/bit-trade-one/BTIRSW-Remote-KawaruKun)

---

## 項目リンク

### [設定ツールダウンロード](#setting-tool-download)【必須】  

### [設定ツール使用方法](#how-to-use-the-setting-tool)
#### ・[赤外線信号の記録](#infrared-signal-recording)
#### ・[ボタン設定](#button-setting)
#### ・[入力パターン設定](#input-pattern-setting)
#### ・[ファームウェアアップデート方法](#firmware-update-method)

### [Q&A](#faq)

---

---

#### Setting tool download
## 設定ツールダウンロード
ダウンロード・展開してお使いください。

・設定ツールv100 __[【クリックでダウンロード】](https://github.com/bit-trade-one/BTIRSW-Remote-KawaruKun/releases/download/v100/RemoteKawaruKun_v100.zip)__

---

#### How to use the setting tool
## 設定ツール使用方法  

設定ツールを起動する前にBTIRSW リモート変わる君自体に赤外線送受信モジュ―ル・外部スイッチなどを接続する必要があります。  
下記画像を参考に接続してください。
![image](https://user-images.githubusercontent.com/85532743/187631525-4bd1715b-d424-4468-9108-6aa7c5a37a56.png)  
[クリックで拡大](https://user-images.githubusercontent.com/85532743/187631525-4bd1715b-d424-4468-9108-6aa7c5a37a56.png)  

ソフトを起動するとこの様な画面が表示されます。  
![image](https://user-images.githubusercontent.com/85532743/187110138-1d444b2b-8fd2-44cc-a9ff-278468a351cc.png)  

リモート変わる君本体をPCと接続すると操作できるようになります。
![image](https://user-images.githubusercontent.com/85532743/187110314-431bd602-04dc-4e8e-96d4-8b42cb8942ef.png)  

---

#### Infrared signal recording
## 赤外線信号の記録  

まず、保存する箇所を選択します。  
保存したい箇所の「No.??」のボタンを押してください。   
ここでは例としてNo.01を選択します。  
![image](https://user-images.githubusercontent.com/85532743/187111258-c002351b-1b92-4853-9db8-3831d4b6a08e.png)  

記録開始をクリックし、赤外線送受信モジュールに向かって記録させたい赤外線リモコン信号などを照射してください。  
![image](https://user-images.githubusercontent.com/85532743/187110543-50f104f5-7c60-4889-b0ea-3ebc61f76657.png)  
![赤外線受信図](https://user-images.githubusercontent.com/85532743/187644281-a98545bf-7552-4c5a-bac0-6ba83775a32a.png)  


信号を送り終えたら記録停止を押してください。
![image](https://user-images.githubusercontent.com/85532743/187110746-b53b850d-15e3-420f-83aa-0100c79dfa6c.png)  

名称横のテキストボックスに付けたい信号名称を記入し、保存を押してください。
![image](https://user-images.githubusercontent.com/85532743/187605776-8e677cc3-976c-4a5d-968c-80a819e62682.png)    

これでNo.1に赤外線信号が保存されました。
![image](https://user-images.githubusercontent.com/85532743/187111338-308121b8-c327-4241-87cd-a8a7238f21e4.png)  

---  

#### button setting
## ボタン設定  

外付けボタン・本体の確認ボタンを押した際の挙動を設定できます。
記憶した赤外線信号を送信するための設定をここでする必要があります。

### ボタン入力仕様

ボタン入力かパターン入力、どちらで信号送信を行うか選択出来ます。
![image](https://user-images.githubusercontent.com/85532743/187604074-49b4b780-5e10-4e56-87b0-b6ad573b4949.png)  

#### ボタン入力 
ボタン入力の場合、ボタンが押された際に記憶した赤外線信号を送信することが出来ます。  
送信する赤外線信号を選択したら「設定」を押して書き込みます。  
![image](https://user-images.githubusercontent.com/85532743/187604833-d115c53e-4558-4940-be51-d04eeb32e4eb.png)  
  
![image](https://user-images.githubusercontent.com/85532743/187604990-6023c72c-64b2-4472-8396-46a1d1427dd9.png)  
  
---
  
#### Input pattern setting
## 入力パターン設定  

![image](https://user-images.githubusercontent.com/85532743/187630098-3f4e6a04-3f83-4236-a7f4-c3fe440e9ab7.png)  
短・長のボタン押しのパターンにより1つのボタンで多数の信号を送信できます。  
パターン入力を選択すると使用できます。  
選択後は「設定」を押して書き込んでください。  

  

![image](https://user-images.githubusercontent.com/85532743/187641064-6ed6715b-0dd4-48a7-9ecf-8b0f96aa4a71.png)  
①パターン入力が設定されている場合、ここでスイッチを押すとパターン入力の確認ができます。  
②こちらに有る時間設定はボタン押しの長短判定基準時間です。  
パターン入力の短押しと長押しの判定はこの値によって決まります。  
時間設定の値が、400msの場合、  
ボタンが押されていた時間が、800ms未満(設定時間x2)で短押し、800ms以上で長押しと判定されます。  
ボタンが押されていない時間が、800ms経過(設定時間x2)でパターン入力終了と判断されます。  

使用するパターンは「入力パターン設定」より設定を行います。  
入力パターン設定のタブに移動すると設定を行えます。  
![image](https://user-images.githubusercontent.com/85532743/187607572-d314243a-988a-4321-a9d8-401def4b4e95.png)  
  
__入力パターン設定タブ__
![image](https://user-images.githubusercontent.com/85532743/187610206-00d15ded-200d-492a-a4fb-2b8f42bb6e95.png)  

①6つまでの短・長のパターンをトリガに赤外線信号を送信できます。  
「無」のアイコンをダブルクリックすると「短」になります。  
`「無」→「短」→「長」→「無」...... `  
これにより入力パターンの設定を行ってください。  

②パターンに名称をつけることも可能です。パターン名称のテキストボックスをクリックすると入力可能です。  

③送信赤外線No.にそのパターンが入力された際に出力する信号を設定します。
  
設定が完了したら下の設定ボタンを押して書き込んでください。

少し下の時間設定の項目内で現在入力されたパターンを表示することが出来ます。


---

#### Firmware update method
## ファームウェアアップデート方法  

2022/9/9現在 ファームウェアアップデート用のファイルは配布されていません。  
アップデートは不要です。

---

## FAQ

## Q:姉妹品の変わる君と同じ接続で使えますか



> ### A:変わる君と本製品リモート変わる君の接続は異なります。

こちらの画像を参考に接続を行ってください。
![image](https://user-images.githubusercontent.com/85532743/187631525-4bd1715b-d424-4468-9108-6aa7c5a37a56.png)  
[クリックで拡大](https://user-images.githubusercontent.com/85532743/187631525-4bd1715b-d424-4468-9108-6aa7c5a37a56.png)  
変わる君と同じ接続をしないでください。
