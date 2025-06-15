# 🔎 Custom Bang Redirector

This project is a minimalistic bang-style search redirector. It lets you define custom "bangs" (like `!gh`, `!yt`, etc.) in a simple `bangs.json` file hosted on GitHub, and redirect users based on their query.

## 🚀 How It Works

- The user adds a custom search engine with the url:  
  `https://exmaple.com?q=`

- WHen the do a search engine search the script:
  1. Loads `bangs.json` from this repository
  2. Parses the `!bang` and the search terms
  3. Redirects to the appropriate search engine or site with the query

## 🧠 Bang Format

Each bang is defined as a key-value pair in `bangs.json`:

```json
{
  "!gh": "https://github.com/search?q=%s",
  "!yt": "https://www.youtube.com/results?search_query=%s",
  "!wiki": "https://en.wikipedia.org/w/index.php?search=%s"
}
```

## 📚 Available Bangs

<!-- BANGS_START -->
- `!gh` → https://github.com/search?q=%s
- `!yt` → https://www.youtube.com/results?search_query=%s
- `!wiki` → https://en.wikipedia.org/w/index.php?search=%s
- `!perp` → https://www.perplexity.ai/search?q=%s
- `!chatgpt` → https://chatgpt.com/?q=%s
- `!chat` → https://chatgpt.com/?q=%s
- `!summary` → https://search.brave.com/search?q=%s&source=llmSuggest&summary=1
- `!youai` → https://you.com/search?q=%s&fromSearchBar=true&tbm=youchat&chatMode=default
- `!phind` → https://www.phind.com/search?q=%s&searchMode=auto&allowMultiSearch=true
- `!felo` → https://felo.ai/search?q=%s
- `!ecoai` → https://www.ecosia.org/chat?q=%s
- `!mistral` → https://chat.mistral.ai/chat?q=%s&mode=ai
- `!mis` → https://chat.mistral.ai/chat?q=%s&mode=ai
- `!g` → https://www.google.com/search?q=%s
- `!s` → https://www.startpage.com/sp/search?query=%s
- `!sp` → https://www.startpage.com/sp/search?query=%s
- `!w` → https://en.wikipedia.org/wiki/Special:Search?search=%s
- `!nixpkgs` → https://search.nixos.org/packages?query=%s
- `!ddg` → https://duckduckgo.com/?q=%s
- `!qw` → https://www.qwant.com/?q=%s&t=web
- `!qwant` → https://www.qwant.com/?q=%s&t=web
- `!leta` → https://leta.mullvad.net/search?q=%s&engine=brave
- `!mj` → https://www.mojeek.com/search?q=%s&theme=dark
- `!mojeek` → https://www.mojeek.com/search?q=%s&theme=dark
- `!mjs` → https://www.mojeek.com/search?q=%s&theme=dark&fmt=summary
- `!sum` → https://www.mojeek.com/search?q=%s&theme=dark&fmt=summary
<!-- BANGS_END -->
