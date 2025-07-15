# SpaceIt Stripe Server

This Express server powers Stripe Checkout for the SpaceIt app.

## Setup

1. Add your Stripe Secret Key to a `.env` file:

```
STRIPE_SECRET_KEY=your_secret_key_here
```

2. Install dependencies:

```
npm install
```

3. Start the server:

```
node server.js
```

## Endpoint

POST `/create-checkout-session`

```json
{
  "address": "123 Elm St",
  "price": 500
}
```