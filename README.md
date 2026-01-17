# Structura Project

> **Mapping the pulse of civil engineering.** > Real-time geospatial intelligence for large-scale construction infrastructure.

---

## 🛰️ Overview

**Structura** is a high-performance open-source intelligence (OSINT) platform designed to track, aggregate, and visualize large-scale construction projects. While the current focus is on **Vinci Construction** and its subsidiaries (Eurovia, Sogea, Freyssinet, etc.), the architecture is built to ingest and normalize construction data from any public procurement source.

---

## 🛠️ Technical Ecosystem

Our stack is chosen for maximum performance, memory safety, and developer ergonomics.

| Layer | Technology | Role |
| :--- | :--- | :--- |
| **Frontend** | **SvelteKit** | Reactive UI and high-performance state management. |
| **Backend** | **Rust (Actix-web)** | Fast, memory-safe API and heavy ETL processing. |
| **Mapping** | **MapLibre GL** | Hardware-accelerated vector tile rendering. |
| **Database** | **PostgreSQL + PostGIS** | Spatial querying and geographic data storage. |
| **Data Ingestion** | **Rust Workers** | Automated scraping and cleaning of government Open Data. |

---

## 📂 Core Repositories

- **[structura-core](https://github.com/structura-io/structura-core)**: The Rust engine. Handles data ingestion from `data.gouv.fr`, geocoding, and serving GeoJSON/Vector tiles.
- **[structura-map](https://github.com/structura-io/structura-map)**: The Svelte-based dashboard. Featuring a custom MapLibre implementation for smooth data visualization.
- **[structura-schema](https://github.com/structura-io/structura-schema)**: Centralized documentation, API specs (OpenAPI), and PostGIS database schemas.

---

## 📡 Data Strategy

Structura reconstructs project maps by cross-referencing multiple public data sources:
1. **DECP (Commande Publique)**: Identifying contracts awarded to construction giants.
2. **BAN (Base Adresse Nationale)**: Precise geocoding of administrative project locations.
3. **Corporate Press Feeds**: Enhancing public data with official project descriptions and media.

---

## 🚀 Vision

Our goal is to provide transparency in the construction sector. By visualizing where and how infrastructure is built, we enable better urban planning analysis and public oversight of major civil engineering works.
