# Web Utility Collection

This repository contains collection of utility for web

## [Translator](translator.html)

It's a wrapper for [google translate](https://translate.google.com) but you can get translation for multiple languages in 1 request. To use this utility, you need to gain [translation API key](https://cloud.google.com/translate/docs/quickstarts).

Parameters

Key | Type | Required | Default Value | Description 
--- | ---- | -------- | ------------- | ------------
`defaultLanguage` | language code | no | 'en' | Default language for source, also for getting supported languages list
`apiKey` | string | yes | empty | Google translate API key
`selectedLanguages` | array of language code | no | empty | Comma separated value of language code. It's used as pre-selected target language.

Language code uses [ISO-639-1 Code](https://cloud.google.com/translate/docs/languages).

Examples:
- simple example: [translator.html?apiKey=YOU_API_KEY](translator.html?apiKey=YOU_API_KEY)
- use english as default source: [translator.html?apiKey=YOU_API_KEY&defaultLanguage=en](translator.html?apiKey=YOU_API_KEY&defaultLanguage=en)
- use english as default source, pre select Russian and Japanese as target languages: [translator.html?apiKey=YOU_API_KEY&defaultLanguage=en&selectedLanguages=ru,ja](translator.html?apiKey=YOU_API_KEY&defaultLanguage=en&selectedLanguages=ru,ja)
