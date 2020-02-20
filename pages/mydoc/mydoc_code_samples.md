---
title: Code samples
tags: [formatting]
keywords: dcode samples syntax highlighting
last_updated: July 3, 2016
datatable: true
summary: "You can use fenced code blocks with the language specified after the first set of backtick fences."
sidebar: mydoc_sidebar
permalink: mydoc_code_samples.html
folder: mydoc
---

## Code Samples

Use fenced code blocks with the language specified, like this:

    ```js
    console.log('hello');
    ````

**Result:**

```js
console.log('hello');
```

For the list of supported languages you can use (similar to `js` for JavaScript), see [Supported languages](https://github.com/jneen/rouge/wiki/list-of-supported-languages-and-lexers).

```py
import requests

def get_liwc_scores(text, api_secret_key, api_key):
    text = text.encode('ascii', 'ignore').decode('utf-8')
    text_repl = text.replace('"', r'\"')
    url = 'https://api-v3.receptiviti.com/v3/api/content'
    headers = {'accept': 'application/json', 'X-API-SECRET-KEY': api_secret_key, 'X-API-KEY': api_key, 'Content-Type': 'application/json'}
    data = "{ \"content_tags\": [ \"string\" ], \"content_handle\": \"string\", \"language\": \"pa_english\", \"content_source\": 0, \"content_date\": \"2020-01-01\", \"recipient_id\": \"string\", \"language_content\": \"" + text_repl + "\"}"
    r = requests.post(url, data=data, headers=headers)
    return r

    text = “paste your text sample here”
    api_secret_key = “paste your api secret key here”
    api_key = “paste your api key here”
    r = get_liwc_scores(text, api_secret_key, api_key)
    r
    ```
