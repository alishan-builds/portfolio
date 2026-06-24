# FurnishCo Price & Stock Alert — n8n Workflow

A live automation that monitors Shopify product prices and 
stock availability every 6 hours.

## How it works
1. Schedule trigger fires every 6 hours
2. Reads tracked products from Google Sheets
3. Fetches live data from Shopify's free product JSON API
4. Compares current price/stock against last known values
5. If anything changed → updates Google Sheet + sends Slack alert
6. If nothing changed → ends silently

## Tools used
- n8n (workflow automation)
- Google Sheets (product tracker)
- Shopify product JSON API (free, no API key needed)
- Slack (real-time alerts)

## Live proof
This workflow is actively running on a real Shopify store.
Screenshot: see portfolio at alishan-builds.github.io/portfolio
