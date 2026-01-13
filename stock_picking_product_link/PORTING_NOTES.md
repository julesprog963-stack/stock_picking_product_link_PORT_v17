# Porting Notes (Odoo 17)

## Files touched
- /home/julio/odoo17-dev/custom_addons/stock_picking_product_link/__manifest__.py
- /home/julio/odoo17-dev/custom_addons/stock_picking_product_link/views/stock_picking_views.xml
- /home/julio/odoo17-dev/custom_addons/stock_picking_product_link/PORTING_NOTES.md

## Changes
- Bumped module version to 17.0.1.0.0 to reflect Odoo 17 port.
- Made the smart button visible only when the picking state is `done` to match the requirement.

## Core validation evidence (Odoo 17)
- View XMLID and button box structure verified in `/home/julio/odoo17-dev/odoo_core/addons/stock/views/stock_picking_views.xml` (record `view_picking_form`, `div` with class `oe_button_box`).
- Field `move_ids_without_package` verified in `/home/julio/odoo17-dev/odoo_core/addons/stock/models/stock_picking.py`.
- Usage of `oe_stat_button` verified in `/home/julio/odoo17-dev/odoo_core/addons/stock/views/stock_picking_views.xml`.
