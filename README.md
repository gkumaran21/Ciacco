# Scoop Queue

QR ordering and pickup for counter-service dessert shops (gelato, waffles, cafés).

Flow: taste at the counter → scan QR → order and pay by UPI → token on the phone → WhatsApp message when it's ready → shop gets a customer list to bring people back.

## Demo

`demo/index.html` is a self-contained, clickable pitch demo. It has no backend and moves no money. Use the three tabs at the top:

1. **Customer:** scan landing page, cup and flavour picker, UPI payment (simulated), live token.
2. **Counter:** order queue that replaces paper bills and numbered plates. Tapping **Mark ready** sends the customer's WhatsApp message (simulated).
3. **Owner:** wait times, orders by hour, top flavours, and a WhatsApp campaign to opted-in customers. The numbers are labelled samples plus whatever you order in the demo.

The strip under the tabs tells the presenter what to tap next. **Start over** resets everything.

To show a different shop, edit `BRAND`, `PRODUCTS` and `FLAVOURS` at the top of the script.
