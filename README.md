# EasyAudioRecorder
Unityエディタ上でマイクの音声をwavファイルで録音するスクリプトです。  
  
主に[EasyMotionRecorder](https://github.com/neon-izm/EasyMotionRecorder)等と併用して、モーションと音声を同時に取る使い方をイメージしています。

# 使用方法
[releases](https://github.com/sh-akira/EasyAudioRecorder/releases)からEasyAudioRecorder.unitypackageをダウンロードしてプロジェクトにインポートしてください。

## セットアップ
1. シーンに`/Assets/EasyAudioRecorder/Prefabs/EasyAudioRecorder.prefab`を配置します
1. **もしシーンにAudioListenerが1つも無ければ(通常はMainCameraに付いています)**、AudioListenerをAdd Componentします

## 録音
1. Unityエディタ上でプレイして、(初期設定では)Rキーを押すと録音開始、Xキーで録音終了になります
1. /Assets/Resources/の中にAudio_yyyy_MM_dd_HH_mm_ss.wavファイルが生成されたら録音完了です。

## 詳細設定
![image](https://user-images.githubusercontent.com/30430584/94350645-2e2bab00-008b-11eb-9f1f-d9dfd6425cc5.png)
- Record Start Key : 録音開始のショートカットキー。デフォルトはR
- Record Stop Key : 録音終了のショートカットキー。デフォルトはX
- Sampling Frequency : 録音サンプリング周波数。44100や48000等を設定します。デフォルトは48000
- Microphone Device : 使用するデバイス。空欄でデフォルトのマイクデバイスを使用します
- Microphone Devices : Unityをプレイ中に使用できるデバイス名一覧が表示されます。Microphone Deviceにコピペするとデバイス選択ができます
- IsRecording : 録音中はチェックが付きます

# 動作環境
Windows 10 64bit, Unity 2018.4.20f1で動作確認しています
