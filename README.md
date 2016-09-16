# ZoeyImport
How to format CSV files so they can be imported into Zoey

Column Header	Description
sku
SKU
A unique value to identify your product. No two products can share the same SKU.
_type
Product Type
simple
configurable
group
bundle
virtual
downloadable
Product Types
name
The name of your product. By default this will also define the URL key and cannot be longer than 60 characters.
Name should always be UNIQUE. Having Duplicate Names causes SEO Issues
short_description
A short description of your product found by the Add to Cart button.
description
A detailed description of your product.
price
The base price of the product, prior to any sales or discounts.
status
Whether or not to show this product in your store.
Enabled = 1
Disabled = 2
tax_class_id
Whether or not to charge tax for this product
Not Taxable/ None = 1
Taxable = 2
visibility
How your customers can find this product.
Catalog and Search = 4
Search Only = 3
Catalog Only = 2
Not Visible Individually = 1
weight
The weight of your product expressed only as a number.
qty
Quantity available to purchase
is_in_stock
If this product is in-stock or not
1 = In Stock
0 = Out of Stock
