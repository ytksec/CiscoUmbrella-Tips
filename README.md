# CiscoUmbrella-Tips
Cisco Umbrellaに関する機能、技術情報をまとめていきます。

## Cisco Umbrella とは

公式サイト  https://www.cisco.com/c/m/ja_jp/umbrella.html

SWG(Secure Web Gateway)製品であリ、主にDNSセキュリティに強みを持つ。  
ライセンスにより、DNSセキュリティのみ、クラウドプロキシへのトンネル等を選択出来る。

### 各ライセンスの概要

| ライセンス  | 概要  |  
| --------  | -------  |  
| DNS Security Essencials  | 端末の危険なDNSリクエストを保護  |
| DNS Security Advantage  | 上記に加え、危険と判断されるサイトをSSL（HTTPS）トラフィックを復号して検査  |
| Secure Internet Gateway (SIG) Essentials  | 上記に加え、セキュア Web ゲートウェイ機能、クラウド提供ファイアウォール機能を提供  |

詳しくはCisco サイトを参照　https://www.cisco.com/c/m/ja_jp/umbrella/packages.html

### エージェントソフト（Roaming Client）対応端末

| OS | 対応可否 | 注意点 |
| ------------- | ------------- | ------------- |
| Windows  | ○  |  |
| Mac  | ○  |  |
| iOS  | ○  | MDM必須  |
| Android  | ○  | MDM必須  |

iOSとAndroidに関してはMDMが無いとプロファイルを配ることが出来ない（ストアからのアプリダウンロードだけではNG）ため、導入の際には注意が必要  
iOSに関してはCSC(Cisco Secuurity Connector)をダウンロードした上でのMDMによるプロファイル配布設定が必要・・[ドキュメント](https://docs.umbrella.com/deployment-umbrella/docs/cisco-security-connectorumbrella-%E3%82%BB%E3%83%83%E3%83%88%E3%82%A2%E3%83%83%E3%83%97-%E3%82%AC%E3%82%A4%E3%83%89)  
Androidに関してはAnyconnectアプリからUmbrellaモジュールのセットアップが必要・・[ドキュメント](https://docs.umbrella.com/deployment-umbrella/docs/umbrella-module-for-anyconnect-android-os)  

