

- Wallet Orders
-  CurrencyAmount 

Object

# CurrencyAmount

An amount of money.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
object CurrencyAmount
```

## Properties

`amount`

`string`

 (Required) 

The monetary amount associated with the currency.

`currency`

`string`

 (Required) 

The ISO 4217 currency code that applies to the monetary amount.

Minimum length: `3`

Maximum length: `3`

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

