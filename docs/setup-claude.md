# Claudeを入れる

!!! info "この章のゴール"
    VSCodeの中で **Claude（クロード）** に日本語で話しかけられる状態になること。
    ここまで来ると、次の Git / GitHub の準備を **Claudeに頼んで** 進められます。

<figure markdown="span">
  ![相棒となるツールを使うイメージ](images/illustrations/design-tools.svg){ width="320" }
  <figcaption>「○○して」とお願いすると、操作を手伝ってくれます</figcaption>
</figure>

Claudeは、**VSCodeの中で日本語でお願いできるAIの相棒**です。
「新しいリポジトリを作って」「この変更を記録して」のように頼むと、操作を代わりに進めてくれます。

```mermaid
flowchart LR
    A[VSCode] --> B[拡張機能で<br/>Claudeを検索]
    B --> C[インストール]
    C --> D[Claudeアカウントで<br/>サインイン]
    D --> E([日本語で頼める 🎉])
```

---

## 1. VSCode拡張として入れる（おすすめ）

1. VSCodeの左側の **拡張機能（四角が4つのアイコン :material-puzzle-outline:）** を開く
2. 検索欄に **`Claude`** と入力する
3. 表示された拡張機能を **インストール（Install）** する
4. 画面の案内に従って、Claudeのアカウントでサインインする

!!! quote "📷 画面キャプチャ枠（あとで差し込み）"
    拡張機能で「Claude」を検索した画面を入れます。
    `![Claude拡張のインストール](images/setup-03-claude.png){ width="700" }`

!!! tip "Node.js などの事前準備は不要です"
    Claude Code の VSCode拡張には、必要なもの（CLI）が **内蔵** されています。
    そのため **Node.js のインストールは不要** です。拡張を入れてサインインすれば、すぐ使えます。
    （`npm install` でCLIを入れる方法だけは Node.js が必要ですが、拡張を使うなら関係ありません。）

!!! info "正確な手順は公式案内を確認"
    Claudeの導入方法は更新されることがあります。最新の手順は、社内の案内または公式ドキュメントを確認してください。
    （会社で配布・利用ルールがある場合は、それに従ってください。）

---

## 2. 使ってみる（お願いの仕方）

入力欄に、**日本語でそのまま** 書けばOKです。命令口調でなくてもかまいません。

```text
このフォルダの中身を教えて。
```

```text
README.md を作って、このプロジェクトの説明を書いて。
```

!!! tip "上手に頼むコツ"
    - **何を・どうしたいか** を1〜2文で書く（例：「この変更を記録して、GitHubに送って」）
    - 分からないときは **「これ何？」と聞く**。用語の説明もしてくれます
    - もっと詳しいコツは → [付録：Claudeの頼み方とMarkdown](appendix.md)

!!! warning "貼り付けてはいけない情報"
    パスワード・APIキー・お客様の個人情報などは、**入力欄に貼らない** でください。
    詳しくは → [AIと安全に付き合う](ai-safety.md)

---

## 3. ターミナルでも使う：CLI版（任意）

VSCodeの拡張だけで十分な人は、ここは **飛ばしてOK** です。
ターミナルから `claude` を直接使いたい人向けに、CLI版も入れられます（**Node.js は不要**）。

=== ":material-apple: Mac / Linux"

    ```bash
    curl -fsSL https://claude.ai/install.sh | bash
    ```

=== ":material-microsoft-windows: Windows（PowerShell）"

    ```powershell
    irm https://claude.ai/install.ps1 | iex
    ```

入れたら、ターミナルで `claude` と打って起動し、初回は画面の案内に従ってログインします。

!!! note "Node.js で入れる方法もある"
    すでに Node.js（18以上）がある人は `npm install -g @anthropic-ai/claude-code` でも入れられます。どれか1つの方法でOKです。

---

## この章のまとめ

- [x] Claude拡張を入れた
- [x] サインインして、日本語で話しかけられた

!!! success "次のステップ"
    相棒がそろいました。最後に、変更の履歴を扱う **Git** と、ネット上の置き場 **GitHub** をつなぎます。
    ここからは、迷ったら **Claudeに頼めば** 進められます。

    👉 [GitとGitHubをつなぐ](setup-git.md)
