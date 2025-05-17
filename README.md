![Mozilla Add-on Version](https://img.shields.io/amo/v/no-google-ai-overview?style=for-the-badge&labelColor=red&link=https%3A%2F%2Faddons.mozilla.org%2Fen-GB%2Ffirefox%2Faddon%2Fno-google-ai-overview)![Mozilla Add-on Downloads](https://img.shields.io/amo/dw/no-google-ai-overview?style=for-the-badge)![Mozilla Add-on Users](https://img.shields.io/amo/users/no-google-ai-overview?style=for-the-badge)


![Static Badge](https://img.shields.io/badge/build-stable-brightgreen?style=for-the-badge&label=BUILD)

![LICENSE-badge](https://img.shields.io/badge/any_text-MIT-blue?style=for-the-badge&label=LICENCE)


# NO-GOOGLE-AI-OVERVIEW
![LOGO](icons/banner.png)

**NO-GOOGLE-AI-OVERVIEW** is an open-source, simple, Ready-to-use extension that disables Google AI Overviews.

This extension sets a custom search engine named `Custom-google`. If you like this project, please give it a star! The code is simple, and you're free to modify it to create your own custom search engine extension for Firefox.

## Installation
- [Get it on Firefox Add-ons](https://addons.mozilla.org/en-GB/firefox/addon/no-google-ai-overview/)

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
- `keyword`: Custom keyword for triggering the search engine or `@google` to over