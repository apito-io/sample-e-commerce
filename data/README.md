# E-commerce Sample Data

This folder contains realistic sample data for the E-commerce Store template:

## Data Structure

```
data/
├── product/        # 40 products with specifications
│   ├── [uuid].json # Individual product files
│   └── relation.json # Product relationships
├── category/       # 10 categories
│   ├── [uuid].json # Individual category files
│   └── relation.json # Category relationships
└── customer/       # 25 customers with addresses
    ├── [uuid].json # Individual customer files
    └── relation.json # Customer relationships
```

## Sample Data Features

### Products (40 records)

- Complete product information with names, descriptions, prices
- SKU codes and stock quantities
- Media galleries for product images
- Specifications with repeated fields
- Geo-location data for store locations
- Category relationships

### Categories (10 records)

- Category hierarchy support
- Featured images for categories
- Parent category relationships
- Product associations

### Customers (25 records)

- Complete customer profiles
- Multiple addresses per customer (billing, shipping)
- Geo-location data for addresses
- Contact information and preferences

## Relationship Format

### Product Relations

```json
{
  "product-uuid": {
    "category": {
      "relation_type": "has_one",
      "id": "category-uuid"
    }
  }
}
```

### Category Relations

```json
{
  "category-uuid": {
    "product": {
      "relation_type": "has_many",
      "ids": ["product-uuid-1", "product-uuid-2"]
    }
  }
}
```

## Geo-Location Features

- Store locations for products
- Customer address coordinates
- Shipping and billing address separation
- GPS coordinates for location-based services

## Data Generation

This data was generated using the Apito Data Generator:

```bash
# Regenerate data
./apito-gen
```

## Statistics

- **Total Files**: 78
- **Products**: 40 with complete specifications
- **Categories**: 10 with hierarchical structure
- **Customers**: 25 with multiple addresses
- **Relationships**: 100% coverage with proper foreign keys
- **UUID Format**: All files use UUID v4 naming
- **Geo Features**: Location data for products and customer addresses

---

**Note**: This demonstrates e-commerce data patterns with product catalogs, customer management, and geo-location features suitable for online stores and marketplaces.
