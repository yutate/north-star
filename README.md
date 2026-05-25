# North Star Studio

**Strategic Alignment Tool for Modern Marketing**

> 生成AIではなく、判断軸を作るAI。

https://yutate.github.io/north-star/

---

## What is this

North Star Studio は、マーケティング施策の「成功定義」を会話から生成する戦略的アライメントツール。

North Star は KPI でも、ミッションステートメントでも、成長スローガンでもない。
**組織が解決を選択する「矛盾」** そのものである。

> "Known but not emotionally chosen."
> "Convenient but not personally meaningful."
> "Frequently seen but rarely remembered."

AIは答えを出さない。AIは、チームがすでに感じていたが言語化できなかった矛盾を、鏡のように映し出す。

---

## Core Philosophy

```
Traditional Marketing Tools    →    North Star Studio
最適化・効率・KPI中心              矛盾・関係性・感情構造中心
答えを出すAI                       問いを研ぐAI
コンサル的出力                     戦略的ミラー
```

---

## Features

### Input
- 自由記述の単一テキスト入力（構造不要）
- 悩み・矛盾・観察・アイデアを話すだけ

### AI Output
1. **AI Interpretation** — Detected Goals / Emotional Friction / Strategic Risks / Core Tension
2. **Strategic Contradiction** — ブランドが抱える根本的矛盾の言語化
3. **Relationship Futures** — 3つの関係性の未来（North Star候補）

各 Option の構成：
- North Star Statement（15〜25文字）
- Relationship Vision（関係性ビジョン）
- Keywords
- Avoid（ブランド固有のトラップ）
- Why This Works

### Export
- **↓ JSON** — タイムスタンプ・入力・全出力を含む履歴ファイル
- **↓ PDF** — 日本語対応（IPA Gothic埋め込み）A4レポート
- **COPY TEXT** — クリップボードへのテキスト出力

### Import
- 過去のJSONを読み込んで出力を再表示
- 再編集モード（inputを復元して再生成）

### Multi-Model
| Model | Key |
|-------|-----|
| Claude Sonnet 4 | Anthropic API Key |
| Gemini 2.5 Flash | Google AI API Key |
| GPT-4o | OpenAI API Key |

---

## Language Rules (Prompt Design)

以下の語彙はプロンプト上で明示的に禁止：

`maximize` `optimize` `ROI` `engagement` `data-driven` `scalable` `conversion` `leverage` `synergy` `personalization at scale`

出力は以下を満たすよう設計：
- Emotionally specific（感情的に具体的）
- Culturally grounded（文化的に根拠がある）
- Brand-specific（このブランド固有）
- Strategically uncomfortable（有益な不快感）

---

## Tech Stack

- Single file HTML + Vanilla JS
- jsPDF 2.5.1（PDF生成）
- IPA Gothic subset（日本語フォント埋め込み、67KB）
- No framework, no build step
- GitHub Pages deploy

---

## Version History

| Version | Summary |
|---------|---------|
| v0.1 | Form-based input, single North Star output |
| v0.2 | Conversation-first UX, 3 proposals |
| v0.3 | Universal scope, multi-model, robust JSON parsing |
| v0.4 | PDF export（日本語対応）, JSON export/import |
| v0.5 | Strategic Contradiction section, Relationship Futures構造、generic language禁止 |

---

## Deploy

```bash
# Termux
cp /sdcard/Download/north-star-studio.html ~/north-star/index.html
cd ~/north-star
git add index.html
git commit -m "vX.X: description"
git push
```

---

## Related Tools

- [Tools Portal](https://yutate.github.io/tools/)
- [Ad Strategy Studio](https://yutate.github.io/ad-strategy-studio/)
- [AdCP Execution Lab](https://yutate.github.io/lab/adcp-exe/)
- [Media Planner](https://yutate.github.io/media-planner/)

---

*Built by Yuta Terachi — 2026*
