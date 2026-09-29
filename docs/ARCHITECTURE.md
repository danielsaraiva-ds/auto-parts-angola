# Architecture baseline

## Core domains
Profiles, vehicle fitment, parts, inventory embedded in parts stock, customer cars, promotions, orders, ratings, manager hierarchy, audit logs and site settings.

## Critical invariants
1. Stock is never negative.
2. A part with stock 0 cannot be ordered.
3. Compatibility is never invented.
4. Customer data is isolated by user id.
5. Manager permissions are enforced server-side.
6. WhatsApp is the payment/order handoff, not a payment gateway.
7. Product records remain after stock reaches zero.

## Supabase
The database project ref vfpwucbdbsxybsaqdywp has been provisioned with RLS-protected tables and manager authorization helpers. The frontend must use only the Supabase publishable key.