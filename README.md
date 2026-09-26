# BRAHUBB Real Store

This package contains:
- `index.html` — customer storefront
- `admin.html` — product/order admin panel
- `supabase-schema.sql` — database tables and starter RLS policies

## What is already implemented
- Unlimited product records through the database
- Product search/category browsing
- Product details
- Cart and quantities
- Customer delivery form
- COD-style order placement
- Order number generation
- Orders saved to Supabase when configured
- Admin product creation
- Admin order list and status updates

## Required setup
1. Create a Supabase project.
2. Open SQL Editor and run `supabase-schema.sql`.
3. Copy your Project URL and anon/public key.
4. Put them into `index.html` where `PASTE_SUPABASE_URL` and `PASTE_SUPABASE_ANON_KEY` appear.
5. Upload `index.html` and `admin.html` to the GitHub Pages repo.
6. Open `admin.html`, enter the same URL/key, and add products.

## Production security
The included admin page is deliberately a simple first version. Before going live with real customer data, add Supabase Auth and restrict admin reads/writes with authenticated admin policies. Never put a Supabase service-role key in frontend code.
