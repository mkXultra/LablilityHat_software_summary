# LablilityHat_software_summary
試作用LablilityHatのソフトウェアまとめページ
ハードの情報は別リポジトリ

## LablilityHatとは
ラズパイのHat  
IFTTTにPUSH送信したり、受信してHat上のLEDを光らせる機能がある

## 目次
1. [実現性調査](#実現性調査)
2. [技術選定](#技術選定)
3. [ソフトウェアアーキテクチャ](#ソフトウェアアーキテクチャ)
4. [ソフトウェア](#ソフトウェア)

### 実現性調査

#### IFTTT連携調査
IFTTTとはwebhookを用いて連携を行う  
1. 送信  
[JS版IFTTTのWEBHOOKキック調査](https://github.com/mkXultra/js_call_ifttt_webhook_api)  
[Rust版IFTTTのWEBHOOKキック調査](https://github.com/mkXultra/rust_call_ifttt_webhook_api)  
1. 受信  
[JS版IFTTTのWEBHOOK受信調査](https://github.com/mkXultra/js_receive_ifttt_webhook)  
[Rust版IFTTTのWEBHOOK受信調査](https://github.com/mkXultra/rust_receive_ifttt_webhook)  

#### RaspberryPiHat用
1. LED  
[JS版LED動作確認](https://github.com/mkXultra/js_mock_v1_led_blink)  
[Rust版LED動作確認](https://github.com/mkXultra/rust_mock_v1_led_blink)  
3. Button  
[未着手]()

### 技術選定
開発言語は、今後のIoT開発のスキルアップを図るためにRustを採用する  
ウェブサーバーのフレームワークはRocketを採用する  
懸念点はrustcのnightlyバージョンでしか動かないため予期しないセキュリティリスクが生まれる可能性があるが、試作用のためそこは無視する  

### ソフトウェアアーキテクチャ

[設計資料](https://github.com/mkXultra/LablilityHat_software_design)

### ソフトウェア

[未着手]()
