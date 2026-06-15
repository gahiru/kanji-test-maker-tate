# 漢字テストメーカー縦 / Vertical Kanji Test Maker

小学校向けの縦書き漢字テスト・読みテストを作るための、単一HTMLファイルのブラウザツールです。
CSVで問題を管理し、漢字テスト、こたえ、読みテストを印刷用PDFとして出力できます。

This is a single-file browser tool for creating printable vertical-layout kanji and reading worksheets for elementary school use.

## 特徴

- 縦書きレイアウトの漢字テストを作成できます
- 同じ10問から、漢字テスト、こたえ、読みテストを出力できます
- CSVの読み込み、編集、保存に対応しています
- PDF保存とブラウザ印刷に対応しています
- 旧横版CSVも読み込めます。縦版で使わない項目は無視されます
- サーバー不要で、`index.html` だけをブラウザで開いて使えます
- 入力した問題データはブラウザ内で処理され、学習者名簿などを外部サーバーへ送信しません

## 想定利用者

- 小学生向けの漢字練習プリントを作る先生
- 家庭学習用の漢字テストを作る保護者
- 既存の横書きテストデータを縦書きプリントに変換したい人

## 使い方

1. `index.html` をブラウザで開きます
2. `CSV読込` から問題データを読み込みます
3. 必要に応じて問題文、タイトル、説明文、フォント設定を調整します
4. `漢字テストPDF保存`、`こたえPDF保存`、`読みテストPDF保存`、または `3つのPDF+CSVを保存` を選びます

サンプルデータは `sample-data/01_春休み復習01_漢字テスト問題データ.csv` にあります。

## 問題データの基本記法

問題文では、テストに出す箇所を `[答え|表示する文字]` の形で書きます。

```text
パン//を[売る。|★うる。]
```

- `//` は文節の区切り記号です。印刷時には表示されません
- 漢字だけを出す問題は四角のマスで表示されます
- `★` を使う問題と読みテストは、かっこ付きの回答欄で表示されます

## 動作確認環境

- Microsoft Edge
- Google Chrome
- Windows 11

## プライバシー

このツールは静的HTMLとして動作します。CSVの読み込み、編集、PDF生成はブラウザ上で行われます。
児童名、クラス情報、独自教材などの個人情報や非公開データを公開リポジトリへ追加しないでください。

## ロードマップ

- READMEとサンプルデータの拡充
- PDF出力の回帰確認手順の整備
- 先生・保護者からの利用フィードバックをIssueで管理
- GitHub Pagesなどで使いやすい公開URLを整備

## 貢献

不具合、改善案、教材作成時の困りごとはIssueで歓迎します。
教育現場や家庭学習での実利用に基づくフィードバックを特に重視しています。

## License

MIT License. See [LICENSE](LICENSE).

---

## English

Vertical Kanji Test Maker is a single-file browser tool for creating printable Japanese kanji worksheets.
It is designed for teachers and parents who need quick vertical-layout kanji tests without a backend service.

### Features

- Creates vertical kanji worksheets for elementary school use
- Generates kanji tests, answer sheets, and reading tests from the same 10 questions
- Loads, edits, and saves CSV data
- Exports printable PDFs
- Runs as a single static HTML file
- Processes worksheet data in the browser without uploading it to a server

### Basic Use

1. Open `index.html` in a browser
2. Load a CSV file
3. Adjust questions, titles, instructions, or font settings
4. Export the kanji test, answer sheet, reading test, or all outputs together

### License

MIT License. See [LICENSE](LICENSE).
