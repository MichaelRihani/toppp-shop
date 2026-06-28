# Sample Public Schema

This is a simplified public schema that shows the shape of Toppp without exposing private implementation details.

## Category

```json
{
  "id": "cat_robot_vacuum",
  "slug": "robot-vacuum",
  "name": "Robot vacuum",
  "aliases": ["robot vacuum cleaner", "roomba alternative"],
  "status": "published",
  "last_reviewed_at": "2026-06-28T00:00:00Z"
}
```

## Product

```json
{
  "id": "prod_example_001",
  "brand": "Example Brand",
  "name": "Example Product",
  "description": "A concise product description for shoppers.",
  "image_url": "https://example.com/product.jpg",
  "specs": {
    "battery_life": "120 minutes",
    "warranty": "1 year"
  }
}
```

## Offer

```json
{
  "id": "offer_example_001",
  "product_id": "prod_example_001",
  "retailer": "Amazon",
  "price": 199.99,
  "currency": "USD",
  "availability": "in_stock",
  "retailer_url": "https://example.com/product",
  "affiliate_url": "https://example.com/product?tag=example",
  "last_checked_at": "2026-06-28T00:00:00Z"
}
```

## Recommendation

```json
{
  "id": "rec_robot_vacuum_value",
  "category_id": "cat_robot_vacuum",
  "bucket": "Best for Most People",
  "product_id": "prod_example_001",
  "primary_offer_id": "offer_example_001",
  "summary": "The best balance of cleaning performance, reliability, and price.",
  "pros": [
    "Strong everyday cleaning",
    "Easy app controls",
    "Good price for the feature set"
  ],
  "cons": [
    "Not the quietest option",
    "May struggle with very high thresholds",
    "Replacement parts add long-term cost"
  ],
  "confidence": "reviewed",
  "status": "published"
}
```

## Event

```json
{
  "event": "retailer_cta_clicked",
  "recommendation_id": "rec_robot_vacuum_value",
  "offer_id": "offer_example_001",
  "destination": "Amazon",
  "created_at": "2026-06-28T00:00:00Z"
}
```

## Notes

Production schemas should include stronger validation, audit logs, feed timestamps, source licensing metadata, and access controls.

