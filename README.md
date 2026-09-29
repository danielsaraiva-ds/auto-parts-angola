# Auto Parts Angola

Independent auto-parts sales platform for Angola.

## Source of truth
- GitHub: danielsaraiva-ds/auto-parts-angola
- Supabase project: auto-parts-angola (ref vfpwucbdbsxybsaqdywp, eu-west-1)
- Frontend: Lovable
- Default language: Portuguese
- Secondary language: English

## Business rules
- Sell only parts currently held in real stock.
- Never allow checkout above available stock.
- Stock 0 remains visible as out of stock; never delete the product automatically.
- Payment is discussed through WhatsApp; no payment gateway.
- Compatibility must be confirmed or explicitly marked as needing confirmation.
- Promo codes: each customer can redeem a code only once; total distinct customers are capped.
- Managers control catalog, stock, prices, settings and manager hierarchy.
- No third-party advertising or fake buttons.

## Security
Supabase RLS is enabled on the current public tables. Service/secret keys must never be shipped to the browser.
