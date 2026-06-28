# Toppp Case Study

Toppp is a prototype shopping answer engine for people who want a fast, trusted answer to: "What should I buy?"

Instead of showing a marketplace grid, sponsored placements, or a long review article, Toppp returns three opinionated recommendations for a product query:

1. Best Budget
2. Best for Most People
3. Best Upgrade

The project explores how AI can improve consumer shopping when it is paired with structured product data, transparent evidence, affiliate disclosure, and human editorial judgment.

## Why This Exists

Shopping online is noisy. Search results are filled with ads, marketplaces optimize for conversion, and review content is often hard to trust. AI can help, but only if it is grounded in fresh product data, clear tradeoffs, and honest limits.

Toppp is designed as an answer layer before checkout:

- Search once.
- See the top three options.
- Understand why each pick won.
- See pros, cons, price, retailer, and affiliate disclosure.
- Click out to a retailer only after the decision is clear.

## Public Demo

Live prototype: [toppp-shop.vercel.app](https://toppp-shop.vercel.app)

Example route: [Best Gaming Desktops](https://toppp-shop.vercel.app/best/gaming-desktop)

Note: The current public demo uses sample editorial data to demonstrate the product experience and data model. Production recommendations would require a formal evidence and review workflow before publication.

## What This Case Study Includes

- [Product Thesis](./PRODUCT_THESIS.md)
- [Architecture](./ARCHITECTURE.md)
- [Trust And Editorial Policy](./TRUST_AND_EDITORIAL_POLICY.md)
- [AI Commerce Readiness](./AI_COMMERCE_READINESS.md)
- [Sample Public Schema](./SAMPLE_PUBLIC_SCHEMA.md)
- [Demo Script](./DEMO_SCRIPT.md)
- [Sample Recommendation JSON](./sample-recommendation.json)

## Product Principles

- No sponsored rankings.
- No ads.
- Affiliate links never change the winner.
- Unsupported searches should say "we have not researched this yet."
- AI can assist research, classification, and summarization, but humans approve live recommendations.
- Product data should be structured enough to support future agentic shopping and checkout surfaces.

## Status

This is a portfolio case study for agentic commerce, trusted shopping, and AI-assisted product decision-making.

It is not the full private implementation repo.

