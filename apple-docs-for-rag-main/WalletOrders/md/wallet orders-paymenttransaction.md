

- Wallet Orders
-  PaymentTransaction 

Object

# PaymentTransaction

The details about a payment transaction.

iOS 17.0+iPadOS 17.0+Mac Catalyst 16.0+macOS 14.0+

``` source
object PaymentTransaction
```

## Properties

`amount`

CurrencyAmount

 (Required) 

The amount of the transaction.

`createdAt`

`date-time`

 (Required) 

The date and time when the framework created the transaction, in RFC 3339 format.

`paymentMethod`

PaymentMethod

 (Required) 

A string that represents the payment, such as a payment pass or card used for the transaction.

`status`

`string`

 (Required) 

The fulfillment status.

Possible Values: `pending, approved, completed, cancelled, failed`

`applePayTransactionIdentifier`

`string`

A string that represents the Apple Pay transaction ID.

`transactionType`

`string`

 (Required) 

The type of transaction.

Possible Values: `purchase, refund`

`receipt`

`string`

The filename of a receipt within the bundle that’s associated with the transaction.

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

object PickupFulfillment

The details of a pickup order.

object Return

The details of a return order.

