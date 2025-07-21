# Malaysia Supply Chain Fragility Index

A data engineering project to monitor and analyze Malaysia's dependency on foreign imports, identify sectoral bottlenecks, and quantify supply chain fragility starting with critical domains such as food, medicine, and electronics.

## Project Overview

Malaysia is deeply connected to global trade networks. While this brings efficiency and scale, it also exposes vulnerabilities in times of geopolitical tensions, pandemics, or export restrictions.

The Malaysia Supply Chain Fragility Index (MY-SCFI) is a data-driven platform that:

- Tracks import dependency across key sectors

- Highlights supply bottlenecks and critical nodes

- Scores sectors based on fragility and resilience

- Enables policy-makers, researchers, and businesses to prepare for disruptions

## Data Sources

1. UN Comtrade – Trade flows of goods by HS Code

2. Department of Statistics Malaysia (DOSM) – National import/export statistics

3. World Bank & IMF – Economic indicators for normalization

4. Industry Reports – Sector-specific supply chain data (food, health, tech)

5. News & Alerts – Web scraping for disruption signals

## Fragility Scoring Model

Each sector is scored using a combination of:

Import Dependency Ratio (IDR) = Imports / Total Domestic Use

Supplier Concentration Index (SCI) = Herfindahl-Hirschman Index of source countries

Disruption Frequency Score (DFS) = News alert frequency or volatility index

Time to Recover (TTR) = Proxy via inventory duration or delivery lead time

Final Index = Weighted composite of IDR + SCI + DFS + TTR

## Folder Structure 

```
my-scfi/
├── data_ingestion/
│   └── fetch_comtrade.py
├── pipeline/
│   ├── transform_imports.py
│   └── dbt_models/
├── analysis/
│   └── fragility_index_calculator.ipynb
├── dashboard/
│   └── app.py
├── data/
│   ├── raw/
│   └── processed/
├── config/
│   └── params.yaml
├── README.md
└── requirements.txt

``` 


## Current Phase
[Done] Project initialized

[Ongoing] Domain research & metric design

[In Progress] Data collection & pipeline setup

[Upcoming] Fragility scoring and dashboard

[Upcoming] Public release & whitepaper


## Potential Extensions

- Regional index (ASEAN Supply Chain Fragility)

- ESG impact overlay (e.g., carbon footprint of fragile links)

- Predictive modeling for shortage risk

- Graph database for supply chain linkages (Neo4j)


## Contributions

Open to domain experts, data engineers, analysts, and policy enthusiasts. Feel free to fork, raise issues, or suggest enhancements.

##  License

MIT License = open for public use and academic exploration. 
