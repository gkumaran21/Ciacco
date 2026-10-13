# Scoop Queue

QR ordering and pickup for counter-service dessert shops (gelato, waffles, cafés).

Flow: taste at the counter → scan QR → order and pay by UPI → track **each item** on the phone → flag a stuck item with one tap → shop gets a customer list to bring people back.

The core problem: a numbered plate tracks the whole order, but food is served item by item. When one of two items arrives, the plate still says "nothing served", so the missing item has no owner and the customer has to chase it.

## Demo

`demo/index.html` is a self-contained, clickable pitch demo. It has no backend and moves no money. Use the three tabs at the top:

1. **Customer:** scan landing page, cup and flavour picker, table number, UPI payment (simulated), and an order page showing each item as served or being made, with a **Still waiting for this?** button on pending items.
2. **Counter:** order queue that replaces paper bills. Each item has its own **Served** button. A customer's "still waiting" tap becomes a red alert at the top with the table number. When every item is out, the screen tells staff to collect the plate.
3. **Owner:** time from payment to fully served, items over 8 minutes, customer follow-ups, a list of stuck items (showing the bottleneck station), orders by hour, top flavours, and a WhatsApp campaign to opted-in customers. The numbers are labelled samples plus whatever you order in the demo.

To replay the lost-item story: order two items, serve only the first at the counter, tap **Still waiting for this?** on the customer screen, then serve it from the red alert.

The strip under the tabs tells the presenter what to tap next. **Start over** resets everything.

To show a different shop, edit `BRAND`, `PRODUCTS` and `FLAVOURS` at the top of the script.

## Ciacco concept version

`demo/ciacco/index.html` is the same demo in Ciacco's name, colours and wordmark style, made to pitch to Ciacco's owner. It is labelled on screen as a concept, not an official Ciacco product, and asks search engines not to index it. It is a complete HTML page: open it directly in a phone browser, or host it on an unlisted link. Don't publish it anywhere public without Ciacco's permission.
