# Order Tracking Dashboard

**[▶ Open the live demo](https://angadamethi1998-hue.github.io/order-tracking-dashboard/)**

A live, customer-facing dashboard for a steel bar manufacturer. It shows order status, production progress and payment due dates for each item (UID). The production version runs password-protected for a European customer and pulls data live from Google Sheets.

> This demo uses **generated sample data**. All customers, orders, UIDs and invoices are fictional, and dates move with today's date.

## What it does
- **Order and UID trace:** order, dispatched and outstanding MT by work order, grade and shipment month, with delay alerts.
- **Production flow per UID:** Cast → Rolling → Heat treatment → Inward → Inspection → Packing → Dispatch, with progress for each step.
- **Payments:** invoice numbers only (no amounts), invoices paid per calendar year, invoices due in the next 5 / 10 / 20 / 30 days, and an alert for invoices due within 5 days.
- **Filters:** work order, grade, shipment month, status, customer article number, project orders, plus free-text search.
- **Live indicator:** a pulsing "Live" badge, auto-refresh every 5 minutes, and light and dark mode.

## How the production version works
- **Data:** the team updates a private Google Sheet (order, PMST production and payment tabs).
- **Security:** a Google Apps Script web service returns the data only after the correct password is entered, and strips invoice amounts first.
- **Front end:** one self-contained HTML/JavaScript page with no frameworks, hosted on static hosting.

## Built with
HTML · CSS · JavaScript · Google Sheets · Google Apps Script · GitHub Pages
