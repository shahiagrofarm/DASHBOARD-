SHAHI AGRO FARM — Business Dashboard Starter

WHAT'S INCLUDED
- dashboard.html: separate business dashboard with sales, estimated profit/loss, order counts, customer counts, recorded browser visits, manual sale/expense entry and CSV export that opens in Excel.
- analytics.js: browser-local visit and order logger.
- Existing SHAHI AGRO FARM website files, patched to load analytics and record locally submitted orders.

IMPORTANT LIMITATION
This is a starter prototype, not a true shared live analytics backend. Static website localStorage is isolated by browser/device. It cannot count all visitors across the internet, synchronize orders to your phone/computer, or securely manage private customer records. The dashboard will only show data captured in the same browser storage context. Do not use the local-only version as the authoritative sales ledger.

HOW TO TEST
1. Extract this ZIP.
2. Serve the folder using a local web server (for example VS Code Live Server) rather than opening individual HTML files directly.
3. Visit order.html and submit a test order with fictional test details.
4. Open dashboard.html in the same browser and same site origin. The order should appear.
5. Use “Download Excel-compatible CSV” to download a report that Excel can open.
6. Delete the test order/data before real use.

TO MAKE IT TRULY CONNECTED / PRODUCTION READY
- Deploy the public site and dashboard on the same domain or subdomain.
- Add a backend API and database (for example Supabase or Firebase) to store orders and events centrally.
- Use authentication and role-based access for dashboard.html; do not expose the admin dashboard publicly without login.
- Track page views with a privacy-aware analytics service or a backend event endpoint.
- Store product cost, delivery, advertising, packaging and other operating expenses to calculate real net profit.
- Payment transaction IDs entered by customers are not proof of payment; verify them against the actual payment account before marking orders paid.
- Do not collect or retain unnecessary customer payment data; secure any information you do keep.

Business calculations
- Sales = non-cancelled order totals.
- Estimated profit = sales minus product cost minus manually entered business expenses.
- Cost defaults to zero until you enter the real product cost per unit. A zero cost makes the profit figure look higher than reality.
- The CSV includes orders, visits and expense records in sections. It is Excel-compatible CSV, not a formatted .xlsx workbook.
