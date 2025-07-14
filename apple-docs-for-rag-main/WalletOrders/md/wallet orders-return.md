

- Wallet Orders
-  Return 

Object

# Return

The details of a return order.

iOS 17.2+iPadOS 17.2+Mac Catalyst 14.2+macOS 14.2+

``` source
object Return
```

## Properties

`returnIdentifier`

`string`

 (Required) 

A unique identifier for the return. This isn’t displayed to the user, and is only used for identifying changes and user notifications.

`status`

`string`

 (Required) 

The status of the return.

Possible Values: `open, onTheWay, processing, issue, completed, cancelled`

`carrier`

`string`

The carrier used to return the products.

`dropOffBy`

`date-time`

The date and time for the product drop-off.

Use `ISO 8601` format.

`initiatedAt`

`date-time`

The date and time for the initated return.

Use `ISO 8601` format.

`lineItems`

`[`LineItem`]`

An array of line items for the customer to return, displayed in the order provided.

`notes`

`string`

Additional information about the return.

`returnedAt`

`date-time`

The return date and time of a product.

Use `ISO 8601` format.

`returnLabel`

`string`

A printable filename of a label within the bundle used to mail the products back. The total size of the bundle must be below 5 MB.

- Supports, `PDF`, `JPG`, and `PNG` labels.

`returnManagementURL`

`uri`

A URL where the customer can manage the return.

`returnNumber`

`string`

The number of the return displayed to the customer.

`statusDescription`

`string`

A localized message describing the return status.

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

object LineItem

An item associated with the order.

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

