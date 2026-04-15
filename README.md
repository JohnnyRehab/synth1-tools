# Synth1.sy1 →.json Converter

Synth1のプリセットファイル `.sy1` を `.json` に変換するツールです。
ブラウザで動くGUI版と、Node.js用のCLI版の両方に対応しています。

仕様参考: [Synth1 パッチデータの構造｜Akihiko YAMAZAWA](https://note.com/yamazawa/n/n1e5b47ae6dca)【161532635336134376†L0-L8】

## Features

- **バージョン自動判定**: v1.07 / v1.10 / v1.12 / v1.13 に対応。不明な場合はv1.13として処理
- **ブラウザGUI**: ドラッグ&ドロップで変換、結果をプレビューしてダウンロード
- **Node.js CLI**: コマンドラインから一括変換も可能
- **パラメータ名マッピング**: 番号→Synth1の正式パラメータ名に変換
- **rawデータ保持**: デバッグ用に `番号:値` のオブジェクトも出力

## Demo
https://johnnyrehab.github.io/synth1-tools/

`index.html` をブラウザで開くだけで使えます。サーバー不要。

## Usage

### ブラウザで使う
1. リポジトリをclone or Download ZIP
2. `index.html` をブラウザで開く
3. `.sy1` ファイルをドラッグ&ドロップ
4. 「.jsonをダウンロード」ボタンで保存
