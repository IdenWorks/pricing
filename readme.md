# Pricing

An open-source registry of SaaS pricing data.

This repository contains **human- and machine-readable pricing information**
for popular software products, maintained via automated checks and community
contributions.

Each product has a single JSON file describing its public pricing.

---

## Repository Structure

```
├── data/
│ ├── github.json
│ ├── linear.json
│ └── ...
├── schema/
│ └── template.json
├── README.md
├── CONTRIBUTING.md
└── LICENSE
```

- `data/`  
  Contains one JSON file per product.  
  The filename should be the lowercase product name (e.g. `github.json`).

- `schema/template.json`  
  Reference schema/template that **all pricing files must follow**.

---

## Data Format

Each pricing file includes:
- Product metadata (name, URL, currency, country)
- Last updated date
- One or more plans
- Support for monthly, yearly, and custom pricing

Example:

```json
{
  "product": "GitHub",
  "url": "https://github.com/pricing",
  "currency": "USD",
  "country": "US",
  "updated_at": "2026-02-01",
  "plans": []
}
```

## Usage

You can directly consume the JSON files from this repository for:

-Pricing comparisons
-Monitoring price changes
-Internal tooling or analytics

## Update Policy

-Pricing data is checked periodically via automated workflows
-If a pricing change is detected, a pull request is opened
-New products are added via pull requests

All changes are reviewed and versioned via Git history.

## Contributing

Contributions are welcome!
Please see CONTRIBUTING.md for guidelines.
