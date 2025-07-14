

- Wallet Orders
-  Barcode 

Object

# Barcode

The details of a barcode for an order.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
object Barcode
```

## Properties

`altText`

`string`

The localized text displayed by the barcode. For example, a human-readable version of the barcode data in case of a scanning failure.

`format`

`string`

 (Required) 

The format of the barcode.

Possible Values: `qr, pdf417, aztec, code128`

`message`

`string`

 (Required) 

The contents of the barcode.

`messageEncoding`

`string`

 (Required) 

The text encoding of the barcode message. Typically this is `iso-8859-1`, but you may specify an alternative encoding if required.

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

object Return

The details of a return order.

