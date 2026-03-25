# CharacterCreator4（CC4）の使用方法
## CC4について
- 研究室のデスクトップ型のMouse PCの「k-lab」アカウントでログインすると、「Reallusion Hub」というアプリがあります。
- アプリ内からCharacter Creator4を開くことができます。
- アカウント
  - ユーザ名：kikuchi_462750
  - メールアドレス：kikuchi@waseda.jp
  - パスワード：icdBL33hN@sZYqW
## CC4でアバターを作成する
- Character Creator4起動
  - Reallusion Hubから開く
- 顔の作成
  - 左のリストから「Headshot v2」を選択
  - 上から「IMAGE」、「AUTO」を選択
  - フォルダから参加者の顔写真をドラック＆ドロップ
- 顔、身体のパラメータを調整
- 衣服の設定
- FBXファイルでエクスポート
  - 「File」→「Export」→「FBX」→「Clothed Character」
  - 以下のように設定してエクスポート
    - エクスポート先は「デスクトップ」→「実験」→「{参加者の群}」→「{参加者のID}」→「アバター」
    <br><img width="814" height="830" alt="image" src="https://github.com/user-attachments/assets/61ba5ed0-b54d-4bcc-9550-fe0da9196a68" />
        <img width="817" height="445" alt="image" src="https://github.com/user-attachments/assets/470743d9-38d0-46fd-bfd0-a798ba46331c" />
## CC4で作成したアバターをUnrealEngineに導入
- UE5のプロジェクトを開く
  - 「デスクトップ」→「実験」→参加者のIDのフォルダ→「Unreal Engine」
- コンテンツブラウザでフォルダを開く
  - 「すべて」→「コンテンツ」→「Characters」→「CharacterCreator4」→参加者のIDのフォルダ
- FBXファイルをインポート
  - 左クリック→「～～（ディレクトリ構造）へインポート」→FBXファイルの位置まで移動→FBXファイルを開く（「～～_Motion.Fbx」でない方）
  - メッセージが出るので、「HQ Shader」を選択して「OK」
  - インポートオプションが出るので以下のように設定して「インポート」
    <img width="451" height="691" alt="image" src="https://github.com/user-attachments/assets/b105287f-2b24-45df-9597-436a66597ccb" />
  　<img width="451" height="466" alt="image" src="https://github.com/user-attachments/assets/c08bea8e-88e5-47ff-8ca9-416a154874fa" />
    <br>これ以下はデフォルトのまま
- 必要に応じてマテリアルを調整する
  - スケルタルメッシュを開く
  - 色の薄い部位はマテリアルを開いて、「マテリアルプロパティのオーバー」→「Blend Mode」→「Translucent」または「Opaque」
