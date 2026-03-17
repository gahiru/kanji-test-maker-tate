# 漢字テストメーカー縦 / Vertical Kanji Test Maker

小学校向けの縦版漢字テスト・読みテストを作るための、単一HTMLファイルのブラウザツールです。  
This is a single-file browser tool for creating printable vertical-layout kanji and reading tests for elementary school use.

## 日本語

### 概要
- 縦レイアウトのテストを作成できます（上半分5問、下半分5問）
- 漢字テストと読みテストの両方に対応しています
- CSVの読込・編集・保存、PDF出力、印刷ができます
- 旧横版CSVも読めます。縦版で未使用の項目は無視されます
- `//` は文節の区切り記号で、印刷時には表示されません

### 動作確認環境
- Microsoft Edge
- Google Chrome
- Windows 11（英語版）

### 使い方
1. `index.html` をブラウザで開きます
2. CSVファイルを読み込みます
3. 必要に応じて問題文や説明文を調整します
4. PDF出力または印刷を行います

### 問題データの基本記法
- 問題は `[答え|テストに出す文字]` の形で入力します
- 固定文字の区切りには `//` を使います
- 例: `パン//を[売る。|★うる。]`

### 練習用データ
- `sample-data/01_春休み復習01_漢字テスト問題データ.csv`

### 公開時の注意
- 公開リポジトリには、個人情報を含むCSVを置かないでください
- 練習用データ以外を追加する場合は、公開してよい内容だけを配置してください

---

## English

### Overview
- Creates vertical worksheet layouts (5 questions in the top half and 5 in the bottom half)
- Supports both kanji tests and reading tests
- Can load, edit, and save CSV data, then export to PDF or print
- Older horizontal-layout CSV files are still supported; unused fields are ignored
- `//` is a phrase separator and is not printed

### Verified environment
- Microsoft Edge
- Google Chrome
- Windows 11 (English)

### Basic use
1. Open `index.html` in your browser
2. Load a CSV file
3. Adjust questions or instructions if needed
4. Export to PDF or print

### Data syntax
- Questions use the format `[answer|text shown in the test]`
- Use `//` to separate fixed text segments
- Example: `パン//を[売る。|★うる。]`

### Practice data
- `sample-data/01_春休み復習01_漢字テスト問題データ.csv`

### Public repository note
- Do not upload CSV files that contain personal information
- Only include sample data that is safe to publish
