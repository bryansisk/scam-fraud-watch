# Search and AI Discovery Architecture

SCAM Watch is designed for standards-based public discovery rather than manipulative ranking tactics.

## Discovery surfaces

- Public HTML pages with descriptive, evidence-specific titles and headings
- Project-site XML sitemap with absolute canonical page URLs
- A project-directory `robots.txt` with permissive crawler examples. **Important:** robots rules only apply when served at the hostname root (`https://bryansisk.github.io/robots.txt`); a file under `/scam-fraud-watch/robots.txt` is not authoritative for crawlers. The project does not control the hostname-root policy through this repository.
- Atom `feed.xml` for update discovery and syndication
- `llms.txt` as a non-standard supplemental navigation aid
- Machine-readable JSON and CSV incident datasets
- Planned stable incident IDs and case URLs (none published yet)
- Category pages and internal links
- Git repository history for transparent revisions

## Notification strategy

Google: sitemap discovery plus Google Search Console ownership/submission when configured. Google states sitemap submission is a discovery hint, not a ranking or indexing guarantee.

IndexNow: once the canonical public host is live and its key is hosted, changed URLs can be submitted to the IndexNow API. Participating search engines share IndexNow notifications. Submission does not guarantee indexing.

AI search: OAI-SearchBot and Anthropic search/user crawlers are permitted. Search inclusion and ranking remain determined by each service.

## Publication rule

Search optimization must never change an evidence classification, invent identifiers, repeat unsupported allegations, expose unnecessary personal data, or use keyword stuffing. Search relevance should come from unique evidence, accurate terminology, stable pages, useful structured data, and legitimate external references.

## Deployment verification

The canonical site and its sitemap must return publicly accessible HTML/XML before indexing claims can be made. Confirm GitHub Pages publishing settings and build status. A valid sitemap in the repository alone does not prove a live Pages deployment. The dataset is currently empty; do not advertise published case reports until an evidence-reviewed record exists.

### October 26, 2026 deployment diagnosis

The official GitHub Pages workflow at `.github/workflows/pages.yml` successfully completed the Jekyll build, including the site's HTML generation. Deployment then stopped at `actions/configure-pages@v5` with `Get Pages site failed: Not Found`. This is consistent with GitHub Pages not yet being enabled or not configured for GitHub Actions in the repository settings. **Do not claim the public website is deployed until the Pages deployment job succeeds and the site URL returns public HTML.**

Repository owner action: open **Settings → Pages → Build and deployment → Source**, choose **GitHub Actions**, and save. Then re-run the **Build and deploy SCAM Watch to GitHub Pages** workflow from the Actions tab. No access token should be pasted into issues or public files. After successful deployment, check the homepage, `sitemap.xml`, and category pages before requesting search indexing.
