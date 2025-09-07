# E-commerce Store - Apito Engine Template

🛒 **A complete e-commerce platform with product catalog, customer management, and geo-location features**

[![Apito Engine](https://img.shields.io/badge/Apito-Engine-blue?style=flat&logo=graphql)](https://apito.io)
[![Project Type](https://img.shields.io/badge/Project%20Type-General-green?style=flat)](#project-type)
[![Models](https://img.shields.io/badge/Models-3-orange?style=flat)](#data-models)
[![Sample Data](https://img.shields.io/badge/Sample%20Data-78%20Files-purple?style=flat)](#sample-data)

## 🚀 Quick Start

1. **Import Schema**: Use `schema.json` to set up your Apito Engine project
2. **Configure Store**: Reference `config.yml` for project metadata
3. **Load Sample Data**: Import the `data/` folder for realistic examples
4. **Customize**: Modify products, categories, and customer fields as needed

## 📋 Project Overview

- **Project Type**: General (Single-tenant)
- **Difficulty Level**: Beginner
- **Category**: E-commerce & Retail

### **Key Features**

- ✅ Product catalog management
- ✅ Category organization
- ✅ Customer management with profiles
- ✅ Geo-location support for addresses
- ✅ Media gallery support
- ✅ Complete sample data

## 🏗️ Data Models

### **🛍️ Product Model** (40 records)

Complete product information with variants, pricing, and media.

**Key Fields:**

- `name`, `description`, `price`, `sku`
- `category_id` (relation to Category)
- `images` (media gallery)
- `inventory_count`, `status`
- `specifications` (object for detailed attributes)

### **📂 Category Model** (10 records)

Product categorization and organization.

**Key Fields:**

- `name`, `slug`, `description`
- `featured_image`, `sort_order`
- Relations to Products

### **👤 Customer Model** (25 records)

Customer profiles with complete information.

**Key Fields:**

- `first_name`, `last_name`, `email`
- `shipping_address`, `billing_address` (geo objects)
- `phone`, `date_of_birth`
- `customer_type`, `status`

## 📊 Sample Data

**78 total files** with realistic e-commerce content:

- **40 Products** - Electronics, clothing, accessories
- **10 Categories** - Electronics, Fashion, Home & Garden, etc.
- **25 Customers** - Complete profiles with addresses

## 🎯 Use Cases

Perfect for building:

- **Online Stores** - Product-based e-commerce
- **Marketplace Platforms** - Multi-vendor support base
- **Inventory Management** - Product tracking systems
- **Customer Databases** - E-commerce customer management

## 🔧 Technical Highlights

- **Geo Fields**: Address locations with coordinates
- **Media Gallery**: Multiple product images
- **Object Fields**: Structured product specifications
- **Relationships**: Product-Category, Customer relationships

## 📦 Installation

```bash
# Clone repository
git clone https://github.com/apito-io/sample-e-commerce

# Import to Apito Engine
apito import schema.json
apito import data/
```

## 🙋‍♂️ Support

- **Documentation**: [Apito Engine Docs](https://docs.apito.io)
- **Issues**: [GitHub Issues](https://github.com/apito-io/sample-e-commerce/issues)
- **Email**: support@apito.io

---

**Built with ❤️ using [Apito Engine](https://apito.io)**
