
---

## 3️⃣ `CONTRIBUTING.md`

```md
# Contributing

Thanks for your interest in contributing to this repository! 🎉  
This project aims to keep SaaS pricing data accurate, structured, and easy to consume.

---

## How to Contribute

### 1. Adding a new product

1. Create a new JSON file in the `data/` folder  
   - Filename must be lowercase: `product-name.json`
   - Example: `notion.json`

2. Use `schema/template.json` as the reference
   - All required fields must be present
   - Follow the same structure as existing files in `data/`

3. Ensure pricing values match the **public pricing page**
   - No internal, leaked, or private pricing data

---

### 2. Updating an existing product

- Update the relevant fields in the product’s JSON file
- Always update the `updated_at` field
- Do not remove historical structure or rename keys arbitrarily

---

## Schema & Validation

- `schema/template.json` defines the expected structure
- If you’re unsure about a field, check similar products in `data/`
- Keep data **explicit** rather than inferred

Examples:
- Use `pricing_type: "custom"` for enterprise/contact-sales plans
- Use `null` for prices that are not publicly listed

---

## Commit Message Guidelines

This repository follows **Conventional Commits**.

Examples:

- `feat(data): add linear pricing`
- `chore(data): update github pricing`
- `fix(data): correct yearly price for linear`
- `docs: improve README`


Common scopes:
- `data`
- `schema`
- `docs`

---

## Pull Requests

- One product per PR is preferred
- Keep diffs clean and focused
- Include a link to the pricing page in the PR description

---

## What Not to Add

- Scraper code
- API tokens or credentials
- Private or negotiated pricing
- HTML snapshots of pricing pages

This repository stores **output data only**.

---

Thanks for contributing! 🚀


