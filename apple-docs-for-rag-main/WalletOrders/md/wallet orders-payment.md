

- Wallet Orders
-  Payment 

Object

# Payment

The payment information associated with the order.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
object Payment
```

## Properties

`total`

CurrencyAmount

 (Required) 

The total amount to be paid.

`summaryItems`

`[`Payment.SummaryItems`]`

A breakdown of the total payment. For example, shipping cost and taxes.

`transactions`

`[`PaymentTransaction`]`

A list of PaymentTransaction dictionaries.

`paymentMethods`

`[string]`

Deprecated 

A list of methods used to pay. For example, MasterCard 1234 or Visa 5678.

`status`

`string`

Deprecated   (Required) 

The status of the payment.

Possible Values: `pending, authorized, paid, refunded, declined, voided`

`applePayTransactionIdentifiers`

`[string]`

Deprecated 

An optional list of Apple Pay transaction identifiers relating to this order. Wallet links the original transaction to your order by default. If you charge a user multiple times, you can provide the relevant transaction identifiers here to enable additional linking.

## Attributes 

Possible types:

## Topics

### Dictionaries

object Payment.SummaryItems

A breakdown of the total payment.

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

