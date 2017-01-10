# ejs_massproduction
EJSとjsonでhtml量産

## バージョン  

### ver 1.0.0

### 使い方と仕様  

#### ＜使い方＞
  1. nodeをインストール
  2. 作業ディレクトリに移動し、コマンド「npm install」で必要なパッケージをインストール
  3. コマンド「gulp」でローカルサーバー起動

#### ＜仕様＞  
  * /src/templates/pages/以下のtemplate.ejsを複製します。  
  data/pages.jsonの数だけhtmlファイルが量産されます。  
  * /src/以下のファイルを編集すると、/src/と同じ階層に「/dist/」フォルダが自動的に生成されます。  
  * ejsのエラーが出ると、/dist/内に「.ejs」のファイルが出力されます。  
  エラーを取り除き、dist内のejsファイルを削除した後、「gulp」コマンドを使用してビルドを行って下さい。
  ＊画像フォルダは/dist内に作成して下さい。  
  例：/dist/images/  
  ＊サーバーにアップロードするのは/dist/内のファイルのみ。
