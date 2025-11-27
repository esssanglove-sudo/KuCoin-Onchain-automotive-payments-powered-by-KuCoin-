KuCoin AutoChain

On-chain automotive payments powered by KuCoin Pay

KuCoin AutoChain is a lightweight payment integration that enables car dealerships and automotive businesses to accept crypto payments through KuCoin Pay.
It provides a simple API flow to create payment orders, generate QR/checkout links, verify payment webhooks, and mark transactions as completed.


---

Features

Create KuCoin Pay payment orders

QR / checkout link generation

Secure webhook verification

One-time, idempotent payment processing

Optional auto-conversion through KuCoin APIs

Clean logs for reconciliation and accounting



---

Use Cases

Full vehicle payments

Reservation deposits

Service & repair payments

Parts and accessories checkout



---

API Endpoints

POST /api/create-payment

Creates a KuCoin Pay order.

Example request:

{
  "orderId": "INV-001",
  "amount": 55000,
  "currency": "USDT"
}

POST /api/webhook/kucoin-pay

Receives and validates KuCoin Pay webhook confirmations.


---

Environment Variables

KUCOIN_API_KEY=
KUCOIN_API_SECRET=
KUCOIN_API_PASSPHRASE=
KUCOIN_WEBHOOK_SECRET=
BASE_URL=
PORT=3000


---

Installation

git clone https://github.com/esssanglove-sudo/kucoin-autochain
cd kucoin-autochain/backend
npm install
npm run dev


---

Project Structure

kucoin-autochain/
 ├── backend/
 │    ├── routes/
 │    ├── utils/
 │    ├── services/
 │    ├── server.js
 │    └── package.json
 ├── README.md
 ├── .env.example


---

For Developers

KuCoin AutoChain provides ready-to-use API logic and webhook handling, making it easy to integrate crypto payments into any automotive or dealership system.


---
