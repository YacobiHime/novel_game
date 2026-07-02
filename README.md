# novel

高専祭で展示予定の新作ノベルゲーム。

将棋の元奨励会員である主人公・戸鎖続と、天性の頭脳を持つヒロイン・天鷺羽音を中心に展開する学園ストーリー。

## 概要

- ジャンル: ノベルゲーム(ADV)
- 使用エンジン: [TyranoScript](https://tyranoscript.com/)
- 展示予定: 高専祭

## キャラクター・プロット

- キャラクター設定: [`characters.md`](./characters.md)
- プロット: [`plot.md`](./plot.md)

## 開発環境のセットアップ

### 1. TyranoScript本体

このリポジトリには、ゲームの実行に必要な TyranoScript 本体(`index.html`, `tyrano/`, `data/`)一式が含まれています。
`index.html` をブラウザで開く(またはローカルサーバー経由で開く)ことでゲームを起動できます。

```bash
# ローカルサーバーを立てて確認する場合
python3 -m http.server 8000
# ブラウザで http://localhost:8000 を開く
```

### 2. ティラノスタジオ(任意・推奨)

シナリオ編集やプレビューを楽にしたい場合は、公式の補助ツール「ティラノスタジオ」を各自のPCにインストールしてください。
これはリポジトリには含めず、開発者ごとに個別にセットアップします。

1. [ティラノスタジオ公式ページ](https://tyrano.jp/studio/) からOSに合ったバージョンをダウンロード
2. 解凍して `TyranoStudio.exe`(Windows)/`TyranoStudio.app`(Mac)を起動
3. 「既存のプロジェクトを読み込む」からこのリポジトリの `index.html` を選択

## ディレクトリ構成

```
novel_game/
├── README.md
├── plot.md              # プロット
├── characters.md         # キャラクター設定
├── index.html            # ゲーム本体
├── tyrano/                # エンジン本体
└── data/
    ├── scenario/          # シナリオファイル(.ks)
    ├── bgimage/            # 背景画像
    ├── fgimage/            # 立ち絵
    ├── bgm/                 # BGM
    └── sound/               # 効果音
```

## シナリオの書き方

シナリオは `data/scenario/` 以下の `.ks` ファイルに記述します。詳しい書き方は [TyranoScript公式ドキュメント](https://tyranoscript.com/) を参照してください。