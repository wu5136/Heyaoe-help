# Content Scorer

A free tool for small store owners and e-commerce writers to check if their product and category page text can be found by AI search engines like ChatGPT, Google AI Overviews, and Perplexity.

No signup. No monthly fee. Paste your text, get a score and a fixed version.

---

## Who this is for

- You run a small online store and write your own product descriptions
- You manage a shop's website but don't have an SEO team
- You want to know why competitors show up in AI search and you don't

---

## What it scores

**AI Visibility** — counts how many sentences in your text can be directly quoted by an AI engine as an answer. A sentence qualifies if it contains a specific fact (a number, size, material, or measurement) and makes sense on its own.

**Search Ranking** — checks whether your keyword appears near the top, whether key product details are covered, and whether there's enough text on the page.

**Easy to Read** — checks sentence length, whether you tell the customer what to do next, and whether any technical terms are left unexplained.

**Trustworthy Facts** — counts specific verifiable details and flags empty marketing words like "best", "amazing", or "premium" used without supporting data.

---

## Does this actually work?

A brake maintenance guide that scored 86 on AI Visibility was confirmed to appear in Google AI Overviews. The guide had 6+ independently quotable sentences covering multiple question types (how to check, how often, what measurements to look for). The scoring logic directly maps to what AI engines extract.

A product selector page with zero specific facts scored 6 on AI Visibility and was not appearing in AI search. Adding three sentences with concrete specs (receiver size, weight rating, install time) was the recommended fix.

The scoring is not a guarantee. It is a signal — high AI Visibility means your text gives AI engines something quotable. Low AI Visibility means there is nothing concrete to quote.

---

## How to use

1. Get a free Anthropic API key at [console.anthropic.com](https://console.anthropic.com/settings/keys). New accounts include enough free credit to run hundreds of scores.
2. Open `index.html` in any browser.
3. Enter your API key, your main keyword, and paste your text.
4. Click **Score my content**.

The tool makes one API call per score. Each call costs roughly $0.01–0.02 USD using Claude Sonnet.

---

## What you get

- A score out of 100 for each dimension
- Inline highlights on your original text showing exactly which sentences are problems and why
- Plain-language fix suggestions for each failing check
- A rewritten version you can copy and use immediately
- Each scoring check links to its public source (Google Search Central, research studies, or foundational documentation)

---

## Scoring sources

Every check is based on publicly documented standards:

| Dimension         | Sources                                                                                                                    |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------- |
| AI Visibility     | Google Search Central — AI Features (Dec 2025) · BrightEdge AI Overviews Study (2025) · Google Passage Indexing (Oct 2020) |
| Search Ranking    | Google Search Essentials · Google BERT (Oct 2019) · Ahrefs Content Length & Rankings study                                 |
| Easy to Read      | Flesch-Kincaid readability (1975) · Nielsen Norman Group · Plain Language Action Network                                   |
| Trustworthy Facts | Google E-E-A-T guidelines (2025) · SearchAtlas AEO study (2025)                                                            |

---

## What this tool does not do

- It does not track whether your page is indexed by Google
- It does not check your site's technical SEO (page speed, mobile, structured data)
- It does not monitor whether you are currently appearing in AI search
- It is not a replacement for a professional SEO audit

For brand-level AI monitoring, see tools like [Profound](https://www.tryprofound.com) or [Peec](https://peec.ai). This tool focuses on the content itself.

---

## Running locally

No build step required. Open `index.html` directly in Chrome, Firefox, or Safari. Your API key is sent directly from your browser to Anthropic and is never stored anywhere.

---

## License

MIT. Free to use, modify, and share.
