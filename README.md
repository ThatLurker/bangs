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
<!-- BANGS_END -->
