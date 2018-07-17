# How to use Anaconda3
## Install
Linux向けのインストーラを以下からダウンロードする。

- https://www.anaconda.com/download/

次に、ダウンロードしたスクリプトを実行して、Anaconda3をインストールする。
```
$ sh Anaconda3-5.2.0-Linux-x86_64.sh
```

## 仮想環境の構築
### 仮想環境の作成
次のコマンドで仮想環境を作成する。
```
$ conda create -n <env_name> <package_spec>
```
Pythonの特定のバージョンや特定のパッケージ入りの環境を作成する場合、次のようにする。
```
$ conda create -n test-env python=3.6 anaconda
```

### 仮想環境の一覧を表示
```
$ conda info -e
```

### 仮想環境の切り替え
作成した仮想環境に入る場合には次のコマンドで、切り替え可能。
```
$ source activate test-env
```
仮想環境を抜ける際には、次のコマンドを実行する。
```
$ source deactivate
```

### 仮想環境の削除
```
$ conda remove -n test-env --all
```
