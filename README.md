# trackings-georgia-courier-api
Georgian courier and parcel tracking API. საქართველოს საკურიერო და ამანათების თრექინგის API. Грузинский API для курьерских и почтовых отправлений.
(Tbilisi, Batumi, Kutaisi).

## 🇬🇧 English
Trackings.ge API provides shipping, tracking, pickup/drop-off, address, and order management in Georgia.  
**Docs:** https://docs.trackings.ge/  
**Swagger:** https://docs.trackings.ge/trackingsge_openapi.yaml  

## 🇬🇪 ქართული
Trackings.ge API გთავაზობთ გადაზიდვის, თრექინგის, პიკაპ/დროფ-ოფის, მისამართებისა და შეკვეთების მართვას.  
**დოკუმენტაცია:** https://docs.trackings.ge/  

## 🇷🇺 Русский
Trackings.ge API предоставляет доставку, отслеживание, пункты приема/выдачи, адреса и управление заказами.  
**Документация:** https://docs.trackings.ge/

This repository is structured for **SEO** and **GEO** discoverability. It includes a clean OpenAPI spec, concise docs, and runnable examples (curl & JavaScript).

## Quick Start

```bash
export BASE_URL="https://trackings.ge/api"
export API_KEY="my_api_key"
```

Example health check:

```bash
curl -s -H "Authorization: Bearer $API_KEY" "$BASE_URL/health"
```

## Repository Structure (strict)
- `openapi/` – canonical spec in YAML and JSON
- `docs/` – domain-focused guides
- `examples/` – ready-to-run `curl/` and `javascript/` requests

## Index
- Orders — `docs/orders.md`
- Addresses — `docs/addresses.md`
- Geography — `docs/geography.md`
- PUDO — `docs/pudo.md`
- Pricing — `docs/pricing.md`
- Invoices — `docs/invoices.md`
