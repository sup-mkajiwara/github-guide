# 基本のIT用語集

パソコンを使うときに出てくる **一般的な言葉** を、身近なたとえで説明します。

!!! tip "読み方"
    全部を覚える必要はありません。「こんな感じ」とイメージがつかめれば十分です。
    前半は **どんな作業でも出てくる基礎用語**、後半は **パソコンを操作するときの言葉** です。

!!! info "このページに載っていない言葉は"
    このページは「**パソコンを使う人なら誰でも出会う言葉**」に絞っています。
    開発の場面で出てくる言葉（API・データベース・デプロイなど）は、まとめて
    [開発の技術用語集](dev-terms.md) にあります。

    - Git/GitHub特有の言葉 → [GitHubの用語集](glossary.md)
    - AI・Claudeの言葉 → [Claudeの用語集](claude-terms.md)

---

## :material-school-outline: 基礎用語（まず知っておきたい）

### :material-file-outline: ファイル（File）
**1つ1つの書類やデータのまとまり** です。文章・画像・プログラムなど、すべてファイルとして保存されます。

> 📄 たとえ：1枚1枚の書類。

### :material-folder: フォルダ（Folder） ／ ディレクトリ（Directory）
**ファイルをまとめて入れておく入れ物** です。ほぼ同じ意味で、**CUIでは「ディレクトリ」と呼ぶことが多い** です。

> 🗂️ たとえ：書類を仕分ける「フォルダ（紙ばさみ）」。

### :material-map-marker-path: パス（Path）
**ファイルやフォルダの「場所（住所）」を表す文字列** です。例：`docs/images/logo.png`。

> 🗺️ たとえ：「○○フォルダの中の△△フォルダの、この書類」という道順。

### :material-file-cog-outline: 拡張子（Extension）
**ファイル名の最後に付く「種類の目印」** です。`.png`＝画像、`.md`＝文章、`.js`＝プログラム、など。

> 🏷️ たとえ：書類の右上に貼った「種類シール」。

### :material-laptop: ローカル ／ :material-cloud-outline: クラウド（オンライン）
- **ローカル** … **自分のPCの中** にある状態。
- **クラウド（オンライン）** … **ネット上** にある状態（GitHubなど）。

> 💻☁️ たとえ：手元の机の上（ローカル）と、ネット上の共有棚（クラウド）。

### :material-link-variant: URL（ユー・アール・エル）
**ネット上の場所を表す「住所」** です。例：`https://github.com/...`。

> 🔗 たとえ：Webページの「番地」。

### :material-web: ブラウザ（Browser）
**Webページを見るためのソフト** です。Chrome・Edge・Safari など。

> 🌐 たとえ：インターネットを見るための「窓」。

### :material-application-outline: アプリ ／ ソフト（Application / Software）
**特定の役割を持つプログラム** のことです。「アプリ」も「ソフト」もほぼ同じ意味。

> 🧰 たとえ：目的別の「道具」。

### :material-download-box-outline: インストール（Install）
**アプリや道具を、自分のPCに入れて使えるようにすること** です。逆に消すのは「アンインストール」。

> 📥 たとえ：道具を箱から出して、使える状態にして棚に置く。

### :material-swap-vertical: ダウンロード ／ アップロード（Download / Upload）
- **ダウンロード** … ネットから **手元に取り込む**。
- **アップロード** … 手元から **ネットへ送り出す**。

> ⬇️⬆️ たとえ：荷物を「受け取る（DL）」か「送る（UL）」か。

### :material-account-circle-outline: アカウント ／ :material-login: ログイン
- **アカウント** … サービスを使うための「自分専用の登録情報」。
- **ログイン（サインイン）** … 「本人です」と確認して入ること。仕組み全体を **認証** と呼びます。

> 🪪🔑 たとえ：サービスごとの「会員証」を見せて中に入る。

### :material-keyboard-variant: ショートカットキー（Shortcut）
**キーの組み合わせで操作を素早く行う方法** です。例：コピーは `Ctrl + C`（Macは `⌘ + C`）。

> ⚡ たとえ：メニューをたどる代わりの「近道」。

---

## :material-console: パソコンを操作する言葉

VSCodeやClaudeを使い始めると出てくる言葉です。最初は読み飛ばしてOK。

### :material-cursor-default-click-outline: GUI（ジー・ユー・アイ）
**画面のボタンやアイコンを、マウスでクリックして操作するやり方** です（Graphical User Interface）。普段のスマホ・パソコンはほぼこれ。

> 🖱️ たとえ：家電のボタンを見て、押したいボタンを指で押すイメージ。

### :material-console: CUI（シー・ユー・アイ） ／ CLI（シー・エル・アイ）
**文字（コマンド）を打ち込んで命令するやり方** です（CUI＝Character／CLI＝Command Line Interface）。ほぼ同じ意味で、**現場では「CLI」と呼ぶことが多い** です。

> ⌨️ たとえ：相手に「○○して」と文章で指示するイメージ。慣れると速く正確に頼める。

| | :material-cursor-default-click-outline: GUI | :material-console: CUI（CLI） |
| :--- | :--- | :--- |
| 操作の方法 | 画面のボタンをクリック | 文字（コマンド）を打つ |
| とっつきやすさ | やさしい・直感的 | 最初は慣れが必要 |
| 得意なこと | かんたんな操作・確認 | 決まった作業を速く・正確に |

!!! success "CUIが苦手でも大丈夫"
    コマンド（CUI）が不安でも、**Claudeに日本語で頼めば代わりに実行してくれます**（→ [Claudeを入れる](setup-claude.md)）。

### :material-console-line: ターミナル（Terminal） ／ :material-code-greater-than: シェル（Shell）
- **ターミナル** … コマンド（CUI）を打ち込むための **画面**。VSCodeにも内蔵。
- **シェル** … そのコマンドを **受け取って実行する中身**（bash・zsh など）。

> 🪟 たとえ：命令を伝える「窓口（ターミナル）」と、その奥で実際に動く「担当者（シェル）」。

### :material-keyboard-outline: コマンド（Command）
**「○○せよ」という1つ1つの命令文** です。例：`gh repo create`（リポジトリを作る命令）。

> 📝 たとえ：作業を頼むときの「短い指示書」。

### :material-application-braces-outline: IDE（アイ・ディー・イー／統合開発環境）
**コードを書く・動かす・直すための道具がひとまとめになったアプリ** です。**VSCodeがその代表**。

> 🛠️ たとえ：文房具・工具が全部そろった「作業デスク」。

---

!!! note "もっと知りたい言葉が出てきたら"
    - 開発で出てくる言葉（API・DB・デプロイなど）→ [開発の技術用語集](dev-terms.md)
    - Git/GitHub特有の言葉 → [GitHubの用語集](glossary.md)
    - AI・Claudeの言葉 → [Claudeの用語集](claude-terms.md)
    - 画面の部品の名前（ボタン・モーダルなど）→ [UI/UXの用語集](ui-vocab.md)
    - 見た目・デザインの言葉 → [デザインの用語集](design-vocab.md)

言葉のイメージがつかめたら、[VSCodeを入れる](setup-vscode.md) に進んで、実際の画面で確かめてみましょう。
