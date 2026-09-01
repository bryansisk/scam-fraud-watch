# Search and AI Discovery Architecture

SCAM Watch is designed for standards-based public discovery rather than manipulative ranking tactics.

## Discovery surfaces

- Public HTML pages with descriptive, evidence-specific titles and headings
- Root XML sitemap with absolute canonical site URLs
- `robots.txt` allowing standard crawlers and explicitly allowing Googlebot, Bingbot, OAI-SearchBot, ChatGPT-User, Claude-SearchBot, Claude-User and ClaudeBot
- Atom `feed.xml` for update discovery and syndication
- `llms.txt` as a non-standard supplemental navigation aid
- Machine-readable JSON and CSV incident datasets
- Stable incident IDs and case URLs
- Category pages and internal links
- Git repository history for transparent revisions

## Notification strategy

Google: sitemap discovery plus Google Search Console ownership/submission when configured. Google states sitemap submission is a discovery hint, not a ranking or indexing guarantee.

IndexNow: once the canonical public host is live and its key is hosted, changed URLs can be submitted to the IndexNow API. Participating search engines share IndexNow notifications. Submission does not guarantee indexing.

AI search: OAI-SearchBot and Anthropic search/user crawlers are permitted. Search inclusion and ranking remain determined by each service.

## Publication rule

Search optimization must never change an evidence classification, invent identifiers, repeat unsupported allegations, expose unnecessary personal data, or use keyword stuffing. Search relevance should come from unique evidence, accurate terminology, stable pages, useful structured data, and legitimate external references.
