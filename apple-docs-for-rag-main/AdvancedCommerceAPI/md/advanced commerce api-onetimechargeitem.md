

- Advanced Commerce API
-  OneTimeChargeItem 

Object

# OneTimeChargeItem

The details of a one-time charge product, including its display name, price, SKU, and metadata.

Advanced Commerce API 1.0+

``` source
object OneTimeChargeItem
```

## Properties

`description`

description

 (Required) 

A description of the product that doesn’t display to customers.

Maximum length: `45`

`displayName`

displayName

 (Required) 

The product name, suitable for display to customers.

Maximum length: `30`

`price`

price

 (Required) 

The price, in milliunits of the currency, of the one-time charge product.

`SKU`

SKU

 (Required) 

The product identifier.

Maximum length: `128`

## Mentioned in 

Creating SKUs for your In-App Purchases

## See Also

### One-time charge creation in the app

object OneTimeChargeCreateRequest

The metadata your app provides when a customer purchases a one-time-charge product.

