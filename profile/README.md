# Gojjam

### **The SQL-Native Ingestion & Orchestration Engine.**

Gojjam enables Analytics Engineers to build, version-control, and scale full-stack data pipelines without leaving their SQL editor.

[**Core Engine**](https://github.com/gojjam-org/gojjam-engine) | [**Quickstart Starter**](https://github.com/gojjam-org/gojjam-starter)

---

## 🚀 The Vision

In the Modern Data Stack, **Data Ingestion remains the final blockade** preventing Analytics Engineers from truly owning the end-to-end data pipeline.

While transformation has been revolutionized by SQL-first tools like dbt, ingestion is still a "gate" guarded by complex Python environments and brittle infrastructure. This creates a dependency cycle where the people who understand the business logic must wait on a dedicated engineering team just to access their data.

**Gojjam tears down this wall.** We treat APIs and SaaS platforms as native relational tables, empowering the Analytics Engineer to be a solo practitioner who owns the entire lifecycle—from raw source to production insight.

## ✨ Key Features

- **SQL-Native Ingestion:** Use standard `SELECT` statements to extract data from REST APIs.
- **Native JSON Flattening:** Query nested JSON objects using simple dot-notation (e.g., `address.street`).
- **Data-as-Code:** 100% Git-integrated. No more clicking through GUIs to manage your pipelines.
- **In-Process Performance:** Powered by a high-speed engine for minimal latency and high-performance extraction.
- **Built for AI:** Architecturally optimized for LLM-assisted code generation—it's easier to prompt SQL than a GUI.

## 🛠️ How it Works

Gojjam bridges the gap between raw API endpoints and your data warehouse.

1.  **Declare:** Define your sources and sinks in simple YAML.
2.  **Select:** Write SQL models to extract and flatten nested data.
3.  **Run:** Execute end-to-end pipelines with a single command: `gojjam run --all`.

```sql
-- An example Gojjam model: No Python, just SQL.
SELECT
    id,
    user.name AS customer_name,
    address.city AS location, -- Automatic JSON extraction
    total_amount
FROM api_source
WHERE status = 'completed'
```

---

## 📦 Repositories

- [**gojjam-engine**](https://github.com/gojjam-org/gojjam-engine): The core open-source engine responsible for extraction, scalar transformation, and orchestration.
- [**gojjam-starter**](https://github.com/gojjam-org/gojjam-starter): A boilerplate project to get your first pipeline running in under 60 seconds with a pre-configured environment.

## 🏢 Beyond Open Source

**Gojjam Cloud** provides a managed platform for production-grade orchestration, observability, and enterprise security. We handle the infrastructure so you can focus on the business logic.

---

_Built with ❤️ in Addis Ababa for the global data community._
