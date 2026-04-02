An AI guide (checked)

### __Confirm which billing account has your education credits__

1. In the Cloud Console, go to Billing → Your billing accounts (the page you’re on).

2. Click each Billing Account for Education row (and “personal” if needed) and look for: 1) The Credits / Transactions section showing an education coupon or promo credit, or 2) Recent Promotional credits line items.

3. Identify the billing account that actually has your remaining education grant balance. That’s the one you use.

4. Make sure your project is linked to that billing account

### Decide which GCP project you want to run Cloud Run in

1. In the console top bar, pick your project selector and switch to the project that should use the credits.

2. In the left nav, go to Billing (within the project context).

 ▫ If you see a message like “This project is not linked to a billing account,” click Link a billing account.

3. Choose the Billing Account for Education that you just confirmed has credits.

4. Click Set account / Link billing. If you have multiple “course” billing accounts (e.g., one for Big Data Programming, one for another course), it’s often simplest to create or use a separate project per course and attach each project to its matching education billing account.

5. Redeem (or re‑redeem) your coupon if you haven’t already

### If you still have an unused coupon email from the faculty program:

1. Open the email and click Redeem now, or go to the “Redeem credits” page in the docs:
2. When prompted, choose to apply it to a new or existing billing account (this usually ends up as something like “Billing Account for Education – [Course Name]”).
3. After redeeming, repeat step 2 above to link your project to this newly redeemed billing account.
4. Verify Cloud Run is actually charging against that account

### Once the project is linked to the correct education billing account:

1. Deploy or update your Cloud Run service in that project.
2. After some traffic, go to Billing → Reports on that billing account.
3. Filter by Project = your Cloud Run project and Service = “Cloud Run” to confirm. As long as the project is tied to the education billing account, Cloud Run usage will consume that credit before any real charges.

### Common gotchas to check

- If Cloud Run won’t deploy because of billing, the project may still be linked to a different billing account (e.g., your “personal” one or an empty course account). Re‑link to the correct one as in step 2.
- Credits are usually valid for 12 months after redemption; if an account shows $0 promo credit, you might need a fresh coupon from the education program. 
