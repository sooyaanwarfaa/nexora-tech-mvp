Nexora Tech — MVP
A working slice of the Nexora Tech platform described in the business plan: QR-based
customer ordering, a cashier queue, a kitchen display, a waiter call-system, and an
admin dashboard for menu/table/staff management. Built with Flask + SQLite so it runs
anywhere with just Python — no external services required.
What's included (Phase 1 / MVP scope)
Customer flow — scan a table's link → browse menu → cart → simulated checkout
(goes through the payment flow described below) → live order-status
page → Call Waiter / Request Bill / Request Water / Assistance.
Cashier dashboard — see new paid orders, view details, send to kitchen, cancel.
Kitchen display — PREPARING → READY → SERVED, grouped by table.
Waiter dashboard — NEW → ACCEPTED → COMPLETED service requests.
Admin dashboard — revenue/order stats, plus full management with Active/Inactive
switches:
Restaurant / hotel details — name, address, phone (name shows on customer menu and staff header)
Menu — add, edit, rename categories, activate/deactivate categories and items, safe delete
(an item that appears in past orders is made inactive instead of deleted)
Tables — add, rename, activate/deactivate, issue a new QR link (old printed QR stops working)
Staff — add, change role, reset password, activate/deactivate (inactive staff are logged out
and can't sign in; you can't deactivate yourself or the last active admin)
Login — session-based auth with hashed passwords, one role per account
(admin / cashier / kitchen / waiter).
