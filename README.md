# trackings-georgia-courier-api
Official API for Trackings.GE. Endpoints for managing orders, addresses, pricing, invoices, and more. Available in KA/EN/RU; covers courier pricing, tracking, COD, express delivery, and PUDO locations across Georgia.

[![Docs](https://img.shields.io/badge/Docs-docs.trackings.ge-informational)](https://docs.trackings.ge/)
[![OpenAPI](https://img.shields.io/badge/OpenAPI-3.0-blue)](https://docs.trackings.ge/trackingsge_openapi.yaml)
[![Developer Portal](https://img.shields.io/badge/Developer%20Portal-trackings.ge%2Fdeveloper--portal-brightgreen)](https://trackings.ge/developer-portal)
[![Shopify App](https://img.shields.io/badge/Shopify-App-black)](https://apps.shopify.com/trackings-ge-courier)
[![CS-Cart Add-on](https://img.shields.io/badge/CS--Cart-Add--on-blue)](https://marketplace.cs-cart.com/trackings-ge-shipping.html)

## EN English
Trackings.GE API provides shipping, tracking, pickup/drop-off, address, and order management in Georgia, for local and international clients.  
**Docs:** https://docs.trackings.ge/  
**Swagger:** https://docs.trackings.ge/trackingsge_openapi.yaml  
**Developer Portal:** https://trackings.ge/en/developer-portal  

## KA ქართული
Trackings.GE API გთავაზობთ გადაზიდვის, თრექინგის, გაცემის პუნქტების, მისამართებისა და შეკვეთების მართვას, როგორც ადგილობრივ ასევე საერთაშორისო კლიენტებს.  
**დოკუმენტაცია:** https://docs.trackings.ge/  
**Swagger:** https://docs.trackings.ge/trackingsge_openapi.yaml  
**დეველოპერების პორტალი:** https://trackings.ge/developer-portal

## RU Русский
Trackings.GE API предоставляет доставку, отслеживание, пункты приема/выдачи, адреса и управление заказами в Грузии, для локальных и международных клиентов.  
**Документация:** https://docs.trackings.ge/  
**Swagger:** https://docs.trackings.ge/trackingsge_openapi.yaml  
**Портал разработчика:** https://trackings.ge/ru/developer-portal  

## 🚀 Features
- **Orders** — create, update, delete, fetch
- **Tracking** — by `order_id`, `uuid`, `tracking_code`, or `client_tracking_code`
- **PUDO** — pickup & drop-off locations across Georgia
- **COD** — cash-on-delivery support & fees
- **Labels & Signatures** — printable labels, sign images
- **Webhooks** — delivery status changes
- **i18n** — `Accept-Language: en | ka | ru`

---

## 🔗 Quick links
- **API Docs (Swagger/OpenAPI):** https://docs.trackings.ge/trackingsge_openapi.yaml  
- **Developer Portal:** https://trackings.ge/developer-portal  
- **Website:** https://trackings.ge/  
- **Shopify App:** https://apps.shopify.com/trackings-ge-courier  
- **CS-Cart Add-on:** https://marketplace.cs-cart.com/trackings-ge-shipping.html  
- **Support:** support@trackings.ge

---

## 🧭 Base URL & Auth
- **Base URL:** `https://trackings.ge`
- **Auth:** `Authorization: Bearer <JWT>`
- **Language (optional):** `Accept-Language: en | ka | ru`
- **Idempotency (optional):** `Idempotency-Key: <uuid>` (safe retries on create)

---

## ✨ Endpoints (overview)
- `POST /api/orders` — Create order  
- `GET /api/orders/{order_id}` — Get order by numeric ID  
- `PUT /api/orders/{order_id}` — Update order (status must be `CREATE`)  
- `DELETE /api/orders/{order_id}` — Delete order (status `CREATE`)  
- `GET /api/orders/lookup?uuid=…|tracking_code=…|client_tracking_code=…` — Lookup by alternate identifiers


