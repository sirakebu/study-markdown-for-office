# Markdownでドキュメントを作成する環境を構築する方法と使い方（VSCode編）

## 1. これはなに？

べいぶが使用しているMarkdownでドキュメントを作成する環境を構築する方法です．
本文には理由を記載せず，手順だけ記載します．

## 2. Index

- [Markdownでドキュメントを作成する環境を構築する方法と使い方（VSCode編）](#markdown%E3%81%A7%E3%83%89%E3%82%AD%E3%83%A5%E3%83%A1%E3%83%B3%E3%83%88%E3%82%92%E4%BD%9C%E6%88%90%E3%81%99%E3%82%8B%E7%92%B0%E5%A2%83%E3%82%92%E6%A7%8B%E7%AF%89%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95%E3%81%A8%E4%BD%BF%E3%81%84%E6%96%B9vscode%E7%B7%A8)
  - [1. これはなに？](#1-%E3%81%93%E3%82%8C%E3%81%AF%E3%81%AA%E3%81%AB)
  - [2. Index](#2-index)
  - [3. 構築方法](#3-%E6%A7%8B%E7%AF%89%E6%96%B9%E6%B3%95)
    - [3.1. VSCode](#31-vscode)
    - [3.2. VSCodeのExtensions](#32-vscode%E3%81%AEextensions)
    - [3.3. VSCodeの設定](#33-vscode%E3%81%AE%E8%A8%AD%E5%AE%9A)
  - [4. ドキュメントの作り方](#4-%E3%83%89%E3%82%AD%E3%83%A5%E3%83%A1%E3%83%B3%E3%83%88%E3%81%AE%E4%BD%9C%E3%82%8A%E6%96%B9)
    - [4.1. Markdown記法](#41-markdown%E8%A8%98%E6%B3%95)
    - [4.2. 目次を作成したいとき](#42-%E7%9B%AE%E6%AC%A1%E3%82%92%E4%BD%9C%E6%88%90%E3%81%97%E3%81%9F%E3%81%84%E3%81%A8%E3%81%8D)
    - [4.3. プレビューを表示したいとき](#43-%E3%83%97%E3%83%AC%E3%83%93%E3%83%A5%E3%83%BC%E3%82%92%E8%A1%A8%E7%A4%BA%E3%81%97%E3%81%9F%E3%81%84%E3%81%A8%E3%81%8D)
    - [4.4. PDF出力したいとき](#44-pdf%E5%87%BA%E5%8A%9B%E3%81%97%E3%81%9F%E3%81%84%E3%81%A8%E3%81%8D)
    - [4.5. テーブルを簡単に作るには](#45-%E3%83%86%E3%83%BC%E3%83%96%E3%83%AB%E3%82%92%E7%B0%A1%E5%8D%98%E3%81%AB%E4%BD%9C%E3%82%8B%E3%81%AB%E3%81%AF)
  - [5. Tips](#5-tips)
    - [5.1. 画像ファイルはどうするのさ！（wikiではなく，ローカルで管理する場合）](#51-%E7%94%BB%E5%83%8F%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%81%AF%E3%81%A9%E3%81%86%E3%81%99%E3%82%8B%E3%81%AE%E3%81%95wiki%E3%81%A7%E3%81%AF%E3%81%AA%E3%81%8F%E3%83%AD%E3%83%BC%E3%82%AB%E3%83%AB%E3%81%A7%E7%AE%A1%E7%90%86%E3%81%99%E3%82%8B%E5%A0%B4%E5%90%88)
    - [5.2. スニペット](#52-%E3%82%B9%E3%83%8B%E3%83%9A%E3%83%83%E3%83%88)
      - [5.2.1. SeeAlso](#521-seealso)
    - [5.3 エディタのフォントが汚いんだけど！](#53-%E3%82%A8%E3%83%87%E3%82%A3%E3%82%BF%E3%81%AE%E3%83%95%E3%82%A9%E3%83%B3%E3%83%88%E3%81%8C%E6%B1%9A%E3%81%84%E3%82%93%E3%81%A0%E3%81%91%E3%81%A9)

## 3. 構築方法

### 3.1. VSCode

[Visual Studio Code \- Code Editing\. Redefined](https://code.visualstudio.com/)[からインストーラをダウンロードします](https://code.visualstudio.com/)からインストーラをダウンロードします)．

インストーラ時のオプションはお好みで良いです．

### 3.2. VSCodeのExtensions

1. VScodeを開く
2. Ctrl + Shift + pででコマンドパレットを開きます
3. "Extensions: Install Extensions"と入力し，Extensionを開きます
4. ”Markdown Preview Enhanced", "Markdown TOC", "Text Tables", "markdownlint"をそれぞれインストールします

### 3.3. VSCodeの設定

1. Ctrl + ,で設定を開きます
2. "Files: Eol"を\r\nにします
3. "markdown-toc.depthFrom"を2にします
4. "Editor: Tab Size"を4にします

## 4. ドキュメントの作り方

1. File -> 新規ファイルの作成で新しいファイルを作成します
2. コマンドパレットで"Change Language Mode"と入力し，言語設定を開きます
3. "Markdown"を選択します．

### 4.1. Markdown記法

[Markdown文法まとめ \- Qiita](https://qiita.com/higuma/items/3344387e0f2cce7f2cfe) を参照ください．

### 4.2. 目次を作成したいとき

1. コマンドパレットで"Markdown Sections: Inserd/Update"を選択します
2. コマンドパレットで"Markdown TOC: Inserd/Update"を選択します

### 4.3. プレビューを表示したいとき

コマンドパレットで"Markdown: Markdown Preview Enhanced: Open Preview”を選択します．

### 4.4. PDF出力したいとき

プレビューを表示し，プレビューを右クリックし，Chrome　(Puppeteer) -> PDFと選択します．

### 4.5. テーブルを簡単に作るには

コマンドパレットを開き，”Text Tables: Enter Table Mode"を選択します

するとExcelと同じような操作感でテーブルが作成できます．

通常の入力モードに戻す場合はコマンドパレットで"Text Tables: Exit TAble Mode"を選択します．

## 5. Tips

### 5.1. 画像ファイルはどうするのさ！（wikiではなく，ローカルで管理する場合）

assetフォルダを作り，そこに保存しています．

```folder tree
hoge/
├ hoge.md
└ asset/
  ├ fuga.jpg
  └ piyo.png
  ```

### 5.2. スニペット

VScodeではスニペットを登録できるので，よく使うテーブルは登録しておくと便利です．

#### 5.2.1. SeeAlso

[Visual Studio Code ユーザースニペットの使い方まとめ | Web-Guided - web業界で働く方を少しだけ手助けするメディア](https://web-guided.com/620/)

### 5.3 エディタのフォントが汚いんだけど！

フォントを変更できますよ！

[VS Codeでフォントを変更するには：Visual Studio Code TIPS \- ](https://www.atmarkit.co.jp/ait/articles/1812/14/news031.html)