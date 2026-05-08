# 🎵 Magical Mirai 2026 — Lyric App

> A synchronized lyric visualization app for Magical Mirai 2026 Programming Contest songs, powered by the TextAlive App API.

---

## ✨ Features

- **Real-time lyric sync** — phrases highlight in time with the music
- **Per-character highlight** — each kanji / kana glows exactly when sung
- **Per-song color themes** — 6 color palettes that shift to match each song's atmosphere
- **Sun / Star visual themes** — toggle between a warm daytime and a dark starfield mode
- **Beat & chord display** — screen pulse + ripple effects on every beat, chord name flashes on screen
- **Equalizer visualizer** — animated bars react while music plays
- **Starfield + binary rain + sunflower petals** — layered ambient background effects
- **Interactive lyrics** — tap/click a character to burst it, double-tap a word to glow the whole word
- **Reaction bar** — fire 🔥 heart ❤️ star ⭐ bolt ⚡ reactions with live counters
- **Vote panel** — vote for your favourite song with a live percentage bar
- **Seekable progress bar** — click or drag (mouse & touch) to seek anywhere in the track
- **Phrase progress bar** — micro-bar shows progress within the current lyric phrase
- **Chorus mode** — enlarged font size for chorus sections
- **Big font toggle** — scale up all lyrics for readability
- **Shake effect** — shake the lyrics with an animation
- **Icon burst mode** — floating FA icons spawn on every phrase change
- **Palette picker** — 6 color accent dots on the left side panel
- **Custom cursor** — smooth trailing ring cursor on desktop
- **Mouse trail** — themed FontAwesome icons follow the cursor
- **Mobile-first responsive** — fluid layout for phones, tablets, and desktops
- **Touch support** — all interactions work on touchscreen (tap, double-tap, swipe, drag)
- **Swipe to toggle theme** — swipe left/right to switch Sun ↔ Star
- **Safe area support** — notch / home indicator aware on modern phones
- **Keyboard shortcuts** — full keyboard control (see below)

---

## 🎶 Songs

| Key | Title | Artist |
|-----|-------|--------|
| 6W2N | こたえて *(Grand Prix)* | imie |
| zoqO | アフター・ザ・カーテン | Rulmry |
| PNpQ | シャッターチャンス | 夜未アガリ |
| B3yJ | 世界最後の音楽隊 | 夏山よつぎ × ど～ぱみん |
| QBdL | トリツクロジー | 鶴三 |
| E2i3 | TAKEOVER | Twinfield |

> **Note:** Only songs published on [Piapro](https://piapro.jp/) with TextAlive lyric data are supported. YouTube or other external links cannot be used because the API requires per-character timing data prepared by the creator on Piapro.

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Space` | Play / Pause |
| `P` | Play |
| `S` | Stop |
| `T` | Toggle Sun / Star theme |
| `E` | Toggle icon burst mode |
| `W` | Shake lyrics |
| `B` | Toggle big font |
| `C` | Toggle chorus mode |
| `R` | Toggle reaction bar |
| `V` | Open vote panel |
| `→` | Seek forward 5 s |
| `←` | Seek backward 5 s |
| `1`–`6` | Switch accent color |

---

## 🚀 Getting Started

Single HTML file — no build step required.

```bash
# Clone the repository
git clone https://github.com/your-username/magical-mirai-2026.git
cd magical-mirai-2026

# Open directly in your browser
open index.html
```

Or just drag `index.html` into any browser.

> **Note:** The TextAlive App API requires an internet connection to load song data and lyrics.

---

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

---

## 🌐 Deployment

**Vercel (recommended)**
1. Push this repository to GitHub
2. Go to [vercel.com](https://vercel.com) → Import your repo
3. Deploy — no configuration needed for a static HTML file

**Netlify**
1. Go to [netlify.com](https://netlify.com) → Drag & drop your `index.html`
2. Done — you'll get a public URL instantly

---

## 🛠 Tech Stack

| Library | Purpose |
|---------|---------|
| [TextAlive App API](https://developer.textalive.jp/) | Lyric sync, beat, chord data |
| [axios](https://axios-http.com/) | HTTP client (TextAlive dependency) |
| [Font Awesome 6](https://fontawesome.com/) | Icons — cursor trail, reactions, UI |
| [Google Fonts](https://fonts.google.com/) | Zen Kurenaido + Noto Serif JP |
| Vanilla JS + Canvas API | Starfield, sunflower petals, binary rain, EQ bars |
| CSS custom properties + `clamp()` | Per-song theming, fluid responsive typography |

---

## 📁 Project Structure

```
magical-mirai-2026/
└── index.html   # Everything in one file — HTML, CSS, JS
```

---

## ⚠️ Notes

- Songs and lyric data are provided by [Piapro](https://piapro.jp/) and TextAlive for the **Magical Mirai 2026 Programming Contest** only
- Adding songs from YouTube or other platforms is **not supported** — the API relies on per-character timing data that only exists for songs registered on Piapro/TextAlive
- Please follow the [TextAlive terms of use](https://developer.textalive.jp/) regarding song data usage

---

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
- **文字単位のハイライト** — 歌われた瞬間に漢字・かながグローします
- **楽曲ごとのカラーテーマ** — 各楽曲の雰囲気に合わせて 6 色のパレットが切り替わります
- **Sun / Star ビジュアルテーマ** — 明るい昼モードとダークな星空モードをトグル切り替え
- **ビート・コード表示** — ビートに合わせて画面パルス＋リップルエフェクト、コード名を表示
- **イコライザービジュアライザー** — 再生中にアニメーションバーが反応します
- **スターフィールド＋バイナリレイン＋ひまわりの花びら** — レイヤード背景エフェクト
- **インタラクティブ歌詞** — 文字をタップでバースト、単語をダブルタップで全文字グロー
- **リアクションバー** — 🔥 ❤️ ⭐ ⚡ リアクションをカウント付きで送信
- **投票パネル** — お気に入りの楽曲に投票、リアルタイムで割合バーを表示
- **シークバー** — クリック・ドラッグ（マウス＆タッチ）で任意の位置にシーク
- **フレーズ進捗バー** — 現在のフレーズ内の進捗をマイクロバーで表示
- **コーラスモード** — サビ区間でフォントを拡大表示
- **ビッグフォントトグル** — 歌詞全体を拡大して読みやすく
- **シェイクエフェクト** — 歌詞をアニメーションで揺らす
- **アイコンバーストモード** — フレーズ切り替え時にフローティング FA アイコンを生成
- **パレットピッカー** — 左サイドパネルの 6 色アクセントドット
- **カスタムカーソル** — デスクトップでスムーズなリングカーソル
- **マウストレイル** — テーマに合った FA アイコンがカーソルを追従
- **モバイルファースト レスポンシブ** — スマートフォン・タブレット・デスクトップに対応
- **タッチ操作対応** — タップ・ダブルタップ・スワイプ・ドラッグがすべて動作
- **スワイプでテーマ切り替え** — 左右スワイプで Sun ↔ Star を切り替え
- **セーフエリア対応** — 最新スマートフォンのノッチ・ホームインジケーターを考慮したレイアウト
- **キーボードショートカット** — フルキーボード操作対応（下表参照）

---

## 🎶 収録楽曲

| キー | タイトル | アーティスト |
|-----|---------|------------|
| 6W2N | こたえて *(グランプリ)* | imie |
| zoqO | アフター・ザ・カーテン | Rulmry |
| PNpQ | シャッターチャンス | 夜未アガリ |
| B3yJ | 世界最後の音楽隊 | 夏山よつぎ × ど～ぱみん |
| QBdL | トリツクロジー | 鶴三 |
| E2i3 | TAKEOVER | Twinfield |

> **注意:** [Piapro](https://piapro.jp/) に TextAlive 歌詞データが登録されている楽曲のみ対応しています。YouTube などの外部リンクは使用できません。API が動作するには Piapro/TextAlive 側でクリエイターが用意した文字単位のタイミングデータが必要なためです。

---

## ⌨️ キーボードショートカット

| キー | 操作 |
|-----|------|
| `Space` | 再生 / 一時停止 |
| `P` | 再生 |
| `S` | 停止 |
| `T` | Sun / Star テーマ切り替え |
| `E` | アイコンバーストモード切り替え |
| `W` | 歌詞シェイク |
| `B` | ビッグフォント切り替え |
| `C` | コーラスモード切り替え |
| `R` | リアクションバー表示 / 非表示 |
| `V` | 投票パネルを開く |
| `→` | 5 秒進む |
| `←` | 5 秒戻る |
| `1`〜`6` | アクセントカラー切り替え |

---

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

---

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

---

## 🌐 デプロイ方法

**Vercel（推奨）**
1. このリポジトリを GitHub にプッシュ
2. [vercel.com](https://vercel.com) → リポジトリをインポート
3. デプロイ — 静的 HTML ファイルなので設定不要です

**Netlify**
1. [netlify.com](https://netlify.com) → `index.html` をドラッグ＆ドロップ
2. 完了 — すぐに公開 URL が発行されます

---

## 🛠 使用技術

| ライブラリ | 用途 |
|-----------|------|
| [TextAlive App API](https://developer.textalive.jp/) | 歌詞同期・ビート・コードデータ |
| [axios](https://axios-http.com/) | HTTP クライアント（TextAlive の依存関係） |
| [Font Awesome 6](https://fontawesome.com/) | アイコン — カーソルトレイル・リアクション・UI |
| [Google Fonts](https://fonts.google.com/) | Zen Kurenaido + Noto Serif JP |
| Vanilla JS + Canvas API | スターフィールド・花びら・バイナリレイン・EQ バー |
| CSS カスタムプロパティ + `clamp()` | 楽曲テーマ・流動的なレスポンシブタイポグラフィ |

---

## 📁 ファイル構成

```
magical-mirai-2026/
└── index.html   # HTML・CSS・JS がすべて 1 ファイルに含まれています
```

---

## ⚠️ 注意事項

- 楽曲・歌詞データは **マジカルミライ 2026 プログラミングコンテスト** 用に [Piapro](https://piapro.jp/) および TextAlive より提供されています
- YouTube などの外部プラットフォームの楽曲は**対応していません** — API の動作には Piapro/TextAlive に登録された文字単位のタイミングデータが必要です
- 楽曲データの利用については [TextAlive の利用規約](https://developer.textalive.jp/) に従ってください

---

## 📄 ライセンス

このプロジェクトのコード部分は MIT ライセンスです。  
楽曲データ・歌詞・音源の著作権は各権利者に帰属します。