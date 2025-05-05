# NO-GOOGLE-AI-OVERVIEW
![LOGO](icons/logo.png)
An open-source, simple-to-use extension that disables Google AI Overviews.

This extension sets a custom search engine named `Custom-google`. If you like this project, please give it a star! The code is simple, and you're free to modify it to create your own custom search engine extension for Firefox.

[Get it on Firefox Add-ons](https://addons.mozilla.org/en-GB/firefox/addon/no-google-ai-overview/)


## How to Use

1. Install the extension from the [Firefox Add-ons store](https://addons.mozilla.org/en-GB/firefox/addon/no-google-ai-overview/).
2. Grant permission to change the default search engine.
3. Done! You can now search without the annoying Google Gemini AI Overviews.

## How It Works

This extension uses `chrome_settings_overrides` to override browser settings in Firefox, Chrome, and Chromium-based browsers.

- `is_default`: Sets this search engine as the default.
- `name`: Name of the custom search engine.
- `search_url`: The URL used for search queries.
  - `{searchTerms}`: This placeholder is replaced with the actual search query by the browser.
- `suggest_url`: URL used for search suggestions.  
  **Note:** The response from this URL must be in JSON format.
  - `{searchTerms}`: This placeholder is replaced with the actual search query by the browser.
- `keyword`: Custom keyword for triggering the search engine or `@google` to override default Google search engine to this.

---

**License :** [MIT LICENSE](./License)

**Made By :** [Junaid](https://abujuni.dev)
