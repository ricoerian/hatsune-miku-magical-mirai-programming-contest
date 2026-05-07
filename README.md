# 🎵 Magical Mirai 2026 — Lyric App

> A synchronized lyric visualization app for Magical Mirai 2026 Programming Contest songs, powered by the TextAlive App API.

---

## ✨ Features

- **Real-time lyric sync** — phrases highlight in time with the music
- **Per-character highlight** — each kanji / kana glows yellow exactly when sung
- **Song themes** — color palette shifts to match each song's atmosphere
- **Beat & chord display** — ripple effects on every beat, chord name flashes on screen
- **Equalizer visualizer** — animated bars react while music plays
- **Starfield + binary rain** — ambient background effects

## 🎶 Songs

| Key | Title | Artist |
|-----|-------|--------|
| 6W2N | こたえて | imie |
| zoqO | アフター・ザ・カーテン | Rulmry |
| PNpQ | シャッターチャンス | 夜未アガリ |
| B3yJ | 世界最後の音楽隊 | 夏山よつぎ × ど～ぱみん |
| QBdL | トリツクロジー | 鶴三 |
| E2i3 | TAKEOVER | Twinfield |

## 🚀 Getting Started

This is a single HTML file — no build step required.

```bash
# Clone the repository
git clone https://github.com/your-username/magical-mirai-2026.git
cd magical-mirai-2026

# Open directly in your browser
open index.html
```

Or just drag `index.html` into any browser.

> **Note:** The TextAlive App API requires an internet connection to load song data and lyrics.

## 🔑 Token Setup

The app uses a [TextAlive App API](https://developer.textalive.jp/) token.

1. Register at [developer.textalive.jp](https://developer.textalive.jp/)
2. Create a new app and copy your token
3. Replace the token value in `index.html`:

```js
app: { token: "YOUR_TOKEN_HERE" }
```

### Restricting your token to your domain

To prevent others from using your token, set **Allowed Origins** in your TextAlive app dashboard to your deployed URL (e.g. `https://your-app.vercel.app`).

## 🌐 Deployment

The easiest way to make this publicly accessible:

**Vercel (recommended)**
1. Push this repository to GitHub
2. Go to [vercel.com](https://vercel.com) → Import your repo
3. Deploy — no configuration needed for a static HTML file

**Netlify**
1. Go to [netlify.com](https://netlify.com) → Drag & drop your `index.html`
2. Done — you'll get a public URL instantly

## 🛠 Tech Stack

| Library | Purpose |
|---------|---------|
| [TextAlive App API](https://developer.textalive.jp/) | Lyric sync, beat, chord data |
| [axios](https://axios-http.com/) | HTTP client (TextAlive dependency) |
| Vanilla JS + Canvas API | Starfield, binary rain, equalizer |
| CSS custom properties | Per-song color theming |

## 📁 Project Structure

```
magical-mirai-2026/
└── index.html   # Everything in one file — HTML, CSS, JS
```

## ⚠️ Notes

- Songs and lyric data are provided by [Piapro](https://piapro.jp/) and TextAlive for the **Magical Mirai 2026 Programming Contest** only
- Please follow the [TextAlive terms of use](https://developer.textalive.jp/) regarding song data usage

## 📄 License

This project (the app code itself) is MIT licensed.  
Song data, lyrics, and audio are property of their respective rights holders.

---

---

# 🎵 Magical Mirai 2026 — 歌詞アプリ

> TextAlive App API を使用した、マジカルミライ 2026 プログラミングコンテスト楽曲対応の歌詞ビジュアライザーアプリです。

---

## ✨ 機能

- **リアルタイム歌詞同期** — 音楽に合わせてフレーズがハイライトされます
- **文字単位のハイライト** — 歌われた瞬間に漢字・かなが黄色くグローします
- **楽曲テーマ** — 各楽曲の雰囲気に合わせてカラーパレットが変わります
- **ビート・コード表示** — ビートに合わせてリップルエフェクト、コード名が画面に表示されます
- **イコライザービジュアライザー** — 再生中にアニメーションバーが反応します
- **スターフィールド + バイナリレイン** — アンビエントな背景エフェクト

## 🎶 収録楽曲

| キー | タイトル | アーティスト |
|-----|---------|------------|
| 6W2N | こたえて *(グランプリ)* | imie |
| zoqO | アフター・ザ・カーテン | Rulmry |
| PNpQ | シャッターチャンス | 夜未アガリ |
| B3yJ | 世界最後の音楽隊 | 夏山よつぎ × ど～ぱみん |
| QBdL | トリツクロジー | 鶴三 |
| E2i3 | TAKEOVER | Twinfield |

## 🚀 使い方

ビルド不要の単一 HTML ファイルです。

```bash
# リポジトリをクローン
git clone https://github.com/your-username/magical-mirai-2026.git
cd magical-mirai-2026

# ブラウザで直接開く
open index.html
```

または `index.html` をブラウザにドラッグ＆ドロップするだけでも動作します。

> **注意:** TextAlive App API は楽曲データ・歌詞の読み込みにインターネット接続が必要です。

## 🔑 トークンの設定

このアプリは [TextAlive App API](https://developer.textalive.jp/) のトークンを使用しています。

1. [developer.textalive.jp](https://developer.textalive.jp/) でアカウントを作成
2. 新しいアプリを作成してトークンをコピー
3. `index.html` 内のトークンを書き換えてください：

```js
app: { token: "YOUR_TOKEN_HERE" }
```

### トークンをドメインに制限する

他のサイトからトークンが使用されないよう、TextAlive アプリのダッシュボードで **Allowed Origins** にデプロイ先の URL（例：`https://your-app.vercel.app`）を設定してください。

## 🌐 デプロイ方法

公開する最も簡単な方法：

**Vercel（推奨）**
1. このリポジトリを GitHub にプッシュ
2. [vercel.com](https://vercel.com) → リポジトリをインポート
3. デプロイ — 静的 HTML ファイルなので設定不要です

**Netlify**
1. [netlify.com](https://netlify.com) → `index.html` をドラッグ＆ドロップ
2. 完了 — すぐに公開 URL が発行されます

## 🛠 使用技術

| ライブラリ | 用途 |
|-----------|------|
| [TextAlive App API](https://developer.textalive.jp/) | 歌詞同期・ビート・コードデータ |
| [axios](https://axios-http.com/) | HTTP クライアント（TextAlive の依存関係） |
| Vanilla JS + Canvas API | スターフィールド・バイナリレイン・イコライザー |
| CSS カスタムプロパティ | 楽曲ごとのカラーテーマ切り替え |

## 📁 ファイル構成

```
magical-mirai-2026/
└── index.html   # HTML・CSS・JS がすべて 1 ファイルに含まれています
```

## ⚠️ 注意事項

- 楽曲・歌詞データは **マジカルミライ 2026 プログラミングコンテスト** 用に [Piapro](https://piapro.jp/) および TextAlive より提供されています
- 楽曲データの利用については [TextAlive の利用規約](https://developer.textalive.jp/) に従ってください

## 📄 ライセンス

このプロジェクトのコード部分は MIT ライセンスです。  
楽曲データ・歌詞・音源の著作権は各権利者に帰属します。