<h1 align="center">のせラジオ（仮）</h1>

<p align="center"><b>直近1週間のニュースから選んだ5〜6本を、<br>キャラクターが読み上げる短い朝のラジオ番組です。</b></p>

<p align="center">
  <a href="https://nemoto1150-spec.github.io/myradio/"><img src="https://img.shields.io/badge/%E2%96%B6%20ON%20AIR-%E3%81%AE%E3%81%9B%E3%83%A9%E3%82%B8%E3%82%AA-ffd028?style=for-the-badge&labelColor=ff4468" alt="のせラジオを聞く"></a>
</p>

- **配信は、台本と音声を置いて push するだけ**。サーバーはいりません（[myradio](https://github.com/monoradio102/myradio) テンプレートで運営）
- 動画ではなく **HTML の番組**です。再生位置に合わせて、スライド・字幕・キャラ・リンクカードが動きます
- ニュースの画像は、記事のサイトがサムネイル用に公開している画像（OGP）をそのサイトから直接表示し、記事へのリンクを添えます。画像を保存したり配り直したりしません
- 選んだニュースは [LEDGER.md](LEDGER.md) に「出来事」単位で記録し、重複して取り上げないようにしています

## 番組について

- カテゴリ： AI・テック／ガジェット／VTuber／金・投資／ノウハウ系／総合トレンド
- 1回あたり約1分30秒〜2分、5〜6本
- 声: COEIROINK:リリンちゃん

## 中身

```
station.json         局の自己紹介
episodes.json        回の一覧
episodes/<日付>-ja.json  台本とタイミング
audio/<日付>-ja.mp3     声（main にはコミットしない。publish.sh が直近30日分だけ gh-pages に載せる）
LEDGER.md            採用した出来事の台帳（重複チェック用）
PROMPTS.md           制作プロンプト集
character/           キャスター
tools/publish.sh     GitHub Pages への公開
```

## ライセンス

- プログラム： MIT License（myradio テンプレート）
- キャラクター（`character/`）： テンプレート同梱のものをそのまま使用（公序良俗に反しない範囲で自由に利用可とされているもの）
- 声： COEIROINK:リリンちゃん（利用規約に従います）
