

- Wallet Orders
-  LineItem 

Object

# LineItem

An item associated with the order.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
object LineItem
```

## Properties

`image`

`string`

The name for an image representing the item.

`price`

CurrencyAmount

The price of the line item.

`quantity`

`number`

 (Required) 

The number of items ordered.

`subtitle`

`string`

A localized secondary display title for the item.

`title`

`string`

 (Required) 

A localized title for the item.

`gtin`

`string`

The Global Trade Item Number of the item, if available. This could be an EAN, ISBN, or other value.

`sku`

`string`

A merchant-specific unique product identifier.

## Attributes 

Possible types:

## See Also

### Supporting objects

object Customer

The details of the order’s customer.

object Merchant

The merchant associated with the order.

object Address

The physical address for an order.

object Application

The details of an app in the App Store.

object Barcode

The details of a barcode for an order.

object CurrencyAmount

An amount of money.

object Location

A geographic location.

object OrderIdentifiers

The unique identifiers associated with orders.

object OrderProvider

Information about the platform providing the order data.

object Payment

The payment information associated with the order.

object Payment.SummaryItems

A breakdown of the total payment.

object PaymentMethod

The payment method for the transaction.

object PaymentTransaction

The details about a payment transaction.

object PickupFulfillment

The details of a pickup order.

object Return

The details of a return order.

