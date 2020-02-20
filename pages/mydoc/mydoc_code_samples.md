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


```curl -X POST "https://api-v3.receptiviti.com/v3/api/content" -H "accept: application/json" 
-H "X-API-SECRET-KEY: Enter your API Secret Key here" -H "X-API-KEY: Enter your API Key here"
-H "Content-Type: application/json" -d "{ \"content_tags\": [ \"string\" ], \"content_handle\": 
\"string\", \"language\": \"English\", \"content_source\": 0, \"content_date\": \"2020-01-01\",
\"recipient_id\": \"string\", \"language_content\": 
\"Enter your language sample here\"}
````
