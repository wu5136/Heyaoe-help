# AI Content Scorer — Free content quality tool for small shops

A free, single-file tool that scores your product or category page content for AI visibility and search quality signals. No signup, no backend, no data stored.

**Live tool:** [wu5136.github.io/Heyaoe-help/category-scorer-v20.html](https://wu5136.github.io/Heyaoe-help/category-scorer-v20.html)

---

## What it does

Paste any product page, category page, or buying guide text. The tool scores it across four dimensions:

| Dimension | What it measures |
|---|---|
| **AI Visibility** | How likely AI engines (ChatGPT, Google AI Overviews, Perplexity) are to quote your page as a direct answer |
| **Search Ranking signals** | Whether your content has the right words and structure for Google to understand it |
| **Easy to Read** | Whether real customers can quickly understand what you're selling and what to do next |
| **Trustworthy Facts** | Whether your content uses specific numbers and details, or vague marketing language |

**Important:** This tool scores your *content quality* — not your actual search ranking. Rankings depend on many factors outside your content (domain authority, backlinks, site speed) that this tool cannot measure.

---

## What's honest about this tool

- **AI Visibility scores correlate with citation likelihood** — we validated this against real content. A brake maintenance guide scoring 86 appeared in Google AI Overviews; a vague product page scoring 6 did not. Correlation, not guarantee.
- **Search Ranking scores reflect content signals only** — a page can have a low content score and still rank highly due to domain authority (see: large established sites). This score is about what you can control: the words on your page.
- **Free scores use a shared API key** — limited to 5 per browser session. After that, you can add your own Anthropic API key.

---

## How to use

### Option A — Use the hosted version (easiest)
Just open the link above. No setup needed.

### Option B — Run your own copy

1. Download `category-scorer-v20.html`
2. Open it in any browser — works locally or hosted

No installation, no dependencies, no server needed.

---

## Cost

The tool uses the Anthropic API (Claude Haiku model).

| Who | Cost per score |
|---|---|
| Using the free demo (first 5 scores) | Free |
| Using your own Anthropic API key | ~$0.02–0.04 per score |

A new Anthropic account comes with free credit — enough for 50–100+ scores before you need to add payment.

> **Previous versions of this README stated ~$0.01 per score.** That was based on the Sonnet model with a longer prompt. The current version uses Haiku with an optimised prompt, which costs approximately $0.02–0.04 per score depending on content length.

---

## Privacy

- 100% runs in your browser
- Your text is sent only to Anthropic to generate the score — not to us
- Your API key is never stored anywhere
- No analytics, no tracking, no cookies

---

## Scoring methodology

Hard metrics (word count, sentence length, keyword position, entity count, Flesch reading ease) are computed locally in JavaScript before the API call. The AI model handles only semantic judgment — it cannot override the pre-computed numbers.

Scoring is based on publicly documented standards:

- **Official:** Google Search Central, Google E-E-A-T guidelines, Plain Language Action Network
- **Research:** BrightEdge AI Overviews Study 2025, Ahrefs content research, Moz on-page SEO
- **Background:** Google BERT, Google Passage Indexing, schema.org

---

## Limitations

- Scores your content text only — not your full page (images, structured data, page speed are not evaluated)
- English and Traditional Chinese supported; other languages may produce inconsistent results
- AI scoring is non-deterministic — the same content may score slightly differently on repeat runs
- Does not evaluate domain authority, backlinks, or any off-page SEO factors

---

## Contributing / Feedback

This is an open-source tool built for small shop owners and content writers who don't have an SEO team. If you have feedback, use the 👍 / 👎 buttons inside the tool, or open a GitHub issue.

---

## License

MIT — free to use, modify, and share.
