# Gradleメモ

### Gradle公式
http://www.gradle.org/

### ドキュメント
http://gradle.monochromeroad.com/docs/

### 始め方
1. 公式からプログラムをダウンロード
2. 環境変数の追加（GRADLE_HOME/bin）
3. 動作確認はgradle -v

### JVMオプション
Gradle実行時に引き渡すJVMオプションは、環境変数GRADLE_OPTSとJAVA_OPTSで設定する。
両方一緒に使うこともできる。

JAVA_OPTSに設定したオプションは、他のJavaアプリケーションで共有されるため、
HTTPプロキシはJAVA_OPTSに設定し、
使用メモリに関する設定はGRADLE_OPTSにセットする、というように使い分ける。

これらの設定はgradleやgradlewスクリプトの**先頭**に記述することも可能。


## Gradleスクリプト

プロジェクトのカレントディレクトリにbuild.gradleを作成し、ビルドスクリプトを記述する。



### 各種疑問

- gradle tasksで表示されるタスクの一覧にないcompileJavaのようなタスクが実行できるのはなぜ？


### 調査ネタ

#### Gradleラッパー
Gradleをインストールせずに実行することのできる仕組みっぽい。
どうやってやるか、準備方法ぐらいを調べておく。
