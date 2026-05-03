# U.S. Bureau of Labor Statistics (u-s-bureau-of-labor-statistics)

The U.S. Bureau of Labor Statistics (BLS) is the principal federal statistical agency responsible for measuring labor market activity, working conditions, and price changes in the U.S. economy. BLS collects, processes, analyzes, and disseminates statistical data on employment, unemployment, inflation, wages, productivity, and occupational safety through a public API that provides programmatic access to published historical time series data.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/u-s-bureau-of-labor-statistics/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Federal Government, Labor, Statistics, Employment, Economic Data

## Timestamps

- **Created:** 2024-12-25
- **Modified:** 2026-05-03

## APIs

### BLS Public Data API

The BLS Public Data API provides programmatic access to published historical time series data covering employment, unemployment, consumer prices, wages, productivity, and other labor market indicators. Version 2 (registration required) supports up to 50 series per request, 20 years of data, and optional calculations including net and percent changes.

**Human URL:** [https://www.bls.gov/developers/](https://www.bls.gov/developers/)

#### Tags:

 - Labor Statistics, Employment, Unemployment, Consumer Prices, Wages

#### Properties

- [Documentation](https://www.bls.gov/developers/api_signature_v2.htm)
- [GettingStarted](https://www.bls.gov/developers/)
- [Authentication](https://data.bls.gov/registrationEngine/)
- [OpenAPI](openapi/bls-public-data-api-openapi.yaml)
- [Series Data Schema](json-schema/bls-series-data-schema.json)
- [Data Point Schema](json-schema/bls-data-point-schema.json)
- [Survey Schema](json-schema/bls-survey-schema.json)
- [Series Data Structure](json-structure/bls-series-data-structure.json)
- [JSON-LD](json-ld/bls-public-data-api-context.jsonld)
- [Series Data Example](examples/bls-series-data-example.json)
- [Data Point Example](examples/bls-data-point-example.json)

## Common Properties

- [Website](https://www.bls.gov/)
- [Documentation](https://www.bls.gov/developers/)
- [GettingStarted](https://www.bls.gov/developers/home.htm)
- [PrivacyPolicy](https://www.bls.gov/bls/bls-privacy.htm)
- [FAQ](https://www.bls.gov/developers/api_faqs.htm)
- [SpectralRules](rules/bls-public-data-api-rules.yml)
- [Vocabulary](vocabulary/u-s-bureau-of-labor-statistics-vocabulary.yaml)
- [Labor Market Intelligence Capability](capabilities/labor-market-intelligence.yaml)

## Features

| Name | Description |
|------|-------------|
| Time Series Data Access | Retrieve historical labor statistics data using BLS series IDs covering employment, unemployment, CPI, wages, and productivity. |
| Multiple Series in One Request | Version 2 API allows requesting up to 50 series in a single POST request, returning 20 years of data per series. |
| Net and Percent Change Calculations | Optional calculations including net change and percent change from prior periods are available in Version 2 responses. |
| Survey Catalog Discovery | Retrieve metadata for all available BLS surveys and discover popular series IDs through the catalog endpoint. |
| Annual Averages | Request annual average values (M13 period) alongside monthly data for trend analysis. |
| Public API with Free Registration | The BLS API is free to use. Version 1 requires no registration; Version 2 requires a free API key for higher query limits. |

## Use Cases

| Name | Description |
|------|-------------|
| Economic Research | Economists and researchers use BLS time series data to analyze labor market trends, wage growth, and employment cycles. |
| Inflation Monitoring | Track CPI and PPI data for measuring inflation trends across consumer goods, food, energy, and other categories. |
| Employment Policy Analysis | Policy analysts use unemployment and employment statistics to evaluate labor market conditions and inform policy decisions. |
| Dashboard and Application Development | Developers integrate BLS data into economic dashboards, journalism applications, and data visualization tools. |
| Academic Research | Universities and think tanks use BLS historical data for econometric modeling, academic papers, and policy reports. |

## Integrations

| Name | Description |
|------|-------------|
| Python blsapi | Open-source Python package for querying the BLS API with support for v1 and v2 endpoints. |
| R blsAPI | CRAN R package providing a simple interface to the BLS Public Data API for statistical computing. |
| Microsoft Power Platform | BLS connector available in Power Automate, Power Apps, and Copilot Studio for low-code BLS data access. |
| data.gov | BLS datasets are cataloged on data.gov as part of the federal open data initiative. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [BLS Public Data API](openapi/bls-public-data-api-openapi.yaml)

### JSON Schema

- [bls-multiple-series-request-schema.json](json-schema/bls-multiple-series-request-schema.json)
- [bls-series-response-schema.json](json-schema/bls-series-response-schema.json)
- [bls-series-results-schema.json](json-schema/bls-series-results-schema.json)
- [bls-series-data-schema.json](json-schema/bls-series-data-schema.json)
- [bls-data-point-schema.json](json-schema/bls-data-point-schema.json)
- [bls-footnote-schema.json](json-schema/bls-footnote-schema.json)
- [bls-series-catalog-schema.json](json-schema/bls-series-catalog-schema.json)
- [bls-calculations-schema.json](json-schema/bls-calculations-schema.json)
- [bls-survey-schema.json](json-schema/bls-survey-schema.json)

### JSON Structure

- [bls-series-data-structure.json](json-structure/bls-series-data-structure.json)
- [bls-data-point-structure.json](json-structure/bls-data-point-structure.json)
- [bls-survey-structure.json](json-structure/bls-survey-structure.json)

### JSON-LD

- [bls-public-data-api-context.jsonld](json-ld/bls-public-data-api-context.jsonld)

### Examples

- [bls-series-data-example.json](examples/bls-series-data-example.json)
- [bls-data-point-example.json](examples/bls-data-point-example.json)
- [bls-survey-example.json](examples/bls-survey-example.json)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [BLS Public Data API](capabilities/shared/bls-public-data-api.yaml) — 5 operations for labor statistics time series access

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Labor Market Intelligence](capabilities/labor-market-intelligence.yaml) | BLS Public Data API | 7 | Economist, Policy Analyst, Data Engineer |

## Vocabulary

- [U.S. Bureau of Labor Statistics Vocabulary](vocabulary/u-s-bureau-of-labor-statistics-vocabulary.yaml) — Unified taxonomy mapping 3 resources, 3 actions, 1 workflow, and 4 personas across labor market data operational and capability dimensions

## Rules

- [BLS Public Data API Spectral Rules](rules/bls-public-data-api-rules.yml) — 30 rules across 13 categories enforcing BLS API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
