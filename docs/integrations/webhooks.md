---
title: Sending your Omnivore data to other apps with Webhooks
editLink: true
---

# {{ $frontmatter.title }}

Omnivore allows you to send your reading data in realtime using webhooks. When a new page is saved or updated, a webhook can be triggered.

Upon setting up the webhook URL, that URL will recieve post requests of the selected webhooks. Here is an example of the body of a POST request for `PAGE_CREATED`

```
{
    "action": "created",
    "userId": "7252931c-4169-11ee-8ce6-83ad71786981",
    "page": {
        "type": "page",
        "userId": "7252931c-4169-11ee-8ce6-83ad71786981",
        "id": "f187586d-1380-4c1b-887f-140fb9217465",
        "slug": "fast-api-experiment-middleware-feature-by-life-is-short-so-enjoy-18a22a66735",
        "originalHtml": "FULLHTML",
        "description": "While I worked on adding authentication into FastAPI application, I had a chance to take a look the FastAPI Middleware feature. Let’s try the example in FastAPI documentation. The example is adding…",
        "title": "FastAPI: Experiment Middleware feature | by Life-is-short--so--enjoy-it | Aug, 2023 | Medium",
        "author": "Life-is-short--so--enjoy-it",
        "url": "https://medium.com/@life-is-short-so-enjoy-it/fastapi-experiment-middleware-feature-c0a0c7314d74",
        "pageType": "ARTICLE",
        "hash": "37e42d0dbd7b710094e77808a81bdd43",
        "image": "https://miro.medium.com/v2/resize:fit:1200/1*SDkMzvL5PNsIGchfG-N--w.png",
        "publishedAt": "2023-08-12T08:05:10.316Z",
        "readingProgressPercent": 0,
        "readingProgressAnchorIndex": 0,
        "state": "SUCCEEDED",
        "createdAt": "2023-08-23T13:47:25.365Z",
        "savedAt": "2023-08-23T13:47:25.365Z",
        "siteName": "Medium",
        "language": "English",
        "siteIcon": "https://miro.medium.com/v2/1*m-R_BkNf1Qjr1YbyOIJY2w.png",
        "wordsCount": 1257,
        "archivedAt": null
    }
}
```

[[toc]]

- [Example of sending your notes to Google Sheets using a Webhook](https://blog.omnivore.app/p/syncing-all-your-notes-to-google)
