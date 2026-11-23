# PriceCharting Scraper - Video Game and Card Prices

Scrape PriceCharting prices for video games, Pokemon cards, TCGs and collectibles: loose, CIB, new, graded PSA 10/9.5/9 values, sales volume and product details by search query, console/set URL or product URL.

**[Run it on Apify Store](https://apify.com/kamerozkan/pricecharting-scraper)**: no servers, no proxies to manage, results as JSON, CSV or Excel, or straight into your app through the API.

## Why use it

- Runs in the cloud on [Apify](https://apify.com/kamerozkan/pricecharting-scraper); start it from the browser, the API, a schedule, or tools like Make, n8n and Zapier.
- Pay only for results. The current price and plan discounts are always on the [Store page](https://apify.com/kamerozkan/pricecharting-scraper).
- Cap the cost of any run with the maximum cost per run setting.

## Quick start

1. Open the [Actor page](https://apify.com/kamerozkan/pricecharting-scraper) and click **Try for free**.
2. Paste an input like the one below and click **Start**.
3. Download the dataset or read it over the API.

```json
{
  "queries": [
    "charizard"
  ],
  "includeDetails": false,
  "maxItems": 20
}
```

## Use it from code

Python ([examples/python_example.py](examples/python_example.py)), Node.js ([examples/node_example.js](examples/node_example.js)) and cURL ([examples/curl.sh](examples/curl.sh)) examples are in the `examples` folder. All of them need an [Apify API token](https://console.apify.com/settings/integrations).

## Use in n8n & Make

- **n8n:** Import [integrations/n8n-workflow.json](integrations/n8n-workflow.json) directly into your n8n workspace, set your `APIFY_TOKEN` environment variable (or Bearer token header), and click **Execute Workflow**.
- **Make / Zapier:** Call the Apify **Run an Actor** module with Actor ID `kamerozkan/pricecharting-scraper` and the JSON input above, or POST to `https://api.apify.com/v2/acts/kamerozkan~pricecharting-scraper/run-sync-get-dataset-items`.

## Use with AI Agents (Apify MCP)

This Actor works with Claude Desktop, Cursor, Windsurf and any MCP-compatible AI agent through the official [Apify MCP Server](https://mcp.apify.com). Copy [integrations/mcp-config.json](integrations/mcp-config.json) into your MCP client configuration and replace `YOUR_APIFY_TOKEN` with your token.

## Sample output

Real rows from a recent run, with any contact details masked. Full sample: [sample-output.json](sample-output.json).

```json
[
  {
    "productId": "6889",
    "name": "Chrono Trigger",
    "consoleOrSet": "Super Nintendo",
    "looseOrUngradedUsd": 270,
    "priceTier2Usd": 799.98,
    "priceTier3Usd": 1642.1,
    "priceLabels": [
      "Loose Price",
      "CIB Price",
      "New Price"
    ],
    "currency": "USD",
    "productUrl": "https://www.pricecharting.com/game/super-nintendo/chrono-trigger",
    "imageUrl": "https://storage.googleapis.com/images.pricecharting.com/rfif6ydrmbugtrol/60.jpg",
    "sourceQuery": "chrono trigger",
    "cibPriceUsd": 799.98,
    "newPriceUsd": 1642.1,
    "scrapedAt": "2026-11-23T10:03:05Z"
  }
]
```

## Support

Found a problem or need a field? Open an issue on the [Actor's Issues tab](https://apify.com/kamerozkan/pricecharting-scraper/issues) and include your run link.

---
This repository holds usage examples and sample data. The Actor itself runs on Apify.
