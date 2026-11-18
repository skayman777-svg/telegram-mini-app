# Telegram Mini App Demo — Bean Coffee

A browser demo of a Telegram Mini App for a coffee shop: menu with search and categories, drink options
(size, milk, syrup) with live price calculation, cart with a promo code, checkout with validation, payment
(card, Telegram Stars, crypto, pay on pickup), order history and status timeline.

**Live demo:** https://skayman777-svg.github.io/telegram-mini-app/

Next to the app the page shows what happens behind the scenes: Telegram WebApp SDK calls
(`ready`, `expand`, `MainButton`, `BackButton`, `openInvoice`, theme events), server API requests,
payment webhooks and the messages the bot sends to the customer.

**This is a demo.** Telegram, the server, payment providers and the bot are simulated on the page;
orders, prices and the address are fictional. In a real project the same UI runs inside Telegram,
the backend verifies `initData`, payments go through Telegram Payments / Stars or a payment provider,
and the bot sends status updates.

Try it: open “Cappuccino”, pick a size and milk, apply promo code `BEAN10` in the cart, place the order
and click “Simulate successful payment”, then watch the status in the bot chat and the event log.

Single `index.html`, no build step, no dependencies.
