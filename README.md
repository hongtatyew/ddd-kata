# ddd-kata

Selling car wash packages
- use mass-transit/carrier
- efcore in-memory
- RESTFUL api
- Solely focus on designing domain and collaboration between micro-services

# DOD
- step by step guide
- recomended solution

#1 product update (admin HTTP POST/PUT) and listings (HTTPGET)
- refer to https://domainmodelling.dev/
- take this as example to start with: car wash packages

#2 add to cart

#3 checkout

#4 membership

#5 appointment

## 7 August 2023

CarWashPackage
- Id
- Name
- Price
- Services
- Validity

CarWashService
- Id
- Name
- Quantity

Promotion
- StartDateTime
- EndDateTime
- Quantity
- DiscountPrice

Direction to design models
1. Strongly type (https://www.youtube.com/watch?v=P5CRea21R2E&t=595s)
2. Invariant

# Scenario
1. One day, one poor John buys a basic car wash package. No promotion.
1. One day, one poor John buys a deluxe car wash package. No promotion.
1. One day, one poor John buys a premium car wash package. No promotion.
2. Promotion day, John buys a basic car wash package with promotion.
2. Promotion day, John buys a deluxe car wash package with promotion.
2. Promotion day, John buys a premium car wash package with promotion.
3. Promotion day, Mary wanted to buy basic car wash package but the promotion package is sold out. Normal price is available.
3. Promotion day, Mary wanted to buy deluxe car wash package but the promotion package is sold out. Normal price is available.
3. Promotion day, Mary wanted to buy premium car wash package but the promotion package is sold out. Normal price is available.
