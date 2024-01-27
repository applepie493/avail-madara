# avail-madara
Madara と Karnot を使用してアプリチェーンをデプロイする方法<br>
avail-Docs<br>
<https://docs.availproject.org/clash-of-nodes/madara-karnot/><br>
Madara-Docs<br>
<https://github.com/karnotxyz/madara-cli?tab=readme-ov-file>

作業フォルダ<br>
$home/avail-madara<br>


## 1.Madara CLI
  ### (1).リポリトジからクローンを作成＆ビルド
  ```
  git clone https://github.com/karnotxyz/madara-cli
  
  ```
  ### (2).依存関係のインストール
  OpenSSLがなかったのでインストール
  ```
  sudo apt-get install libssl-dev
  export PKG_CONFIG_PATH=/usr/lib/pkgconfig
  ```
  ### (3).新しいアプリチェーンの初期化
  ```
  ./target/release/madara init
  ```
  ### (4).実行
  ```
  screen -S madara
  ./target/release/madara run
  ```
  ### (5).エクスプローラーの起動
  ```
  screen -S explorer
  ./target/release/madara explorer
  ```

