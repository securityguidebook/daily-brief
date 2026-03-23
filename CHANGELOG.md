# Changelog — daily-brief

All notable changes to the Daily Brief frontend will be documented here.
Format: `[version] - YYYY-MM-DD — description`

---

## [1.0.2] - 2026-03-23
### Fixed
- `ReferenceError: Cannot access 'tldrGlobalOn' before initialization` — moved variable declarations for `tldrGlobalOn` and `tldrEuOn` above the `loadingPhrases` array that references them
- Worker URL placeholder `YOUR_NAME` replaced with actual deployed Worker subdomain `pgtmk101`

---

## [1.0.1] - 2026-03-23
### Fixed
- File renamed from `daily briefing agent` (no extension, spaces) → `daily-briefing-agent.html` to allow GitHub Pages to serve it correctly
- Repo renamed from `Daily-Brief` → `daily-brief` to fix case-sensitive GitHub Pages URL

---

## [1.0.0] - 2026-03-23
### Added
- Initial release of the Daily Brief frontend
- Newspaper-style layout using Playfair Display + DM Sans typography
- Topic chip toggles: Cybersecurity, AI & ML, Geopolitics, Tech industry, Science, Markets, NZ news, AU news
- Custom topics / keywords input field
- Exclude topics input field
- Depth selector: Headline / Standard / Deep Dive
- TLDR News sources section with toggles for TLDR Global and TLDR EU
- Optional personal context textarea
- Loading state with rotating phrases
- Briefing output rendered from markdown to styled HTML
- Regenerate button
- Error display box
- Calls Cloudflare Worker (`/generate`) instead of Anthropic API directly — API key never exposed in frontend
- Hosted on GitHub Pages at `https://securityguidebook.github.io/daily-brief/daily-briefing-agent.html`
