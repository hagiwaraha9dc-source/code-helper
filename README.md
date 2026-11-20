[README_公開手順.md](https://github.com/user-attachments/files/35173359/README_.md)
# code helper（スマホアプリ版）を公開する手順

このフォルダの中身を GitHub Pages に置くと、スマホにアプリとしてインストールできます。

## 1. GitHub にリポジトリを作る（PC 推奨）
1. https://github.com にログインし、右上の「＋」→「New repository」。
2. Repository name に `code-helper` と入力。
3. **Public** を選ぶ（無料で GitHub Pages を使うには Public が必要です。API キーなどの秘密はファイルに含まれていません）。
4. 「Create repository」。

## 2. ファイルをアップロード
1. 作ったリポジトリの画面で「uploading an existing file」をクリック。
2. このフォルダの中身を**まとめてドラッグ**します。
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `icons` フォルダ（中の png ごと）
   - この README は入れなくても大丈夫です。
3. 下の「Commit changes」。

## 3. GitHub Pages を有効にする
1. リポジトリの「Settings」→ 左の「Pages」。
2. 「Build and deployment」の Source を **Deploy from a branch**、Branch を **main** と **/ (root)** にして「Save」。
3. 1〜2分待つと、`https://（あなたのID）.github.io/code-helper/` で開けるようになります。

## 4. スマホにインストール（Android）
1. Chrome で上の URL を開く。
2. 右上の「⋮」→「アプリをインストール」（または「ホーム画面に追加」→「インストール」）。
3. ホーム画面のアイコンから起動すると、アドレスバーのないアプリとして開きます。

## 5. Gemini を設定
1. https://aistudio.google.com/apikey で「Create API key」を押してキーを作る（無料）。
2. アプリの「AI」ボタン →「Gemini」→ キーを貼り付け →「接続テスト」。
   - キーはそのスマホのブラウザ内にだけ保存されます。

## 更新するとき
新しいファイルを同じようにアップロードして上書きすれば、次にアプリを開いたときに自動で新しい版になります。
