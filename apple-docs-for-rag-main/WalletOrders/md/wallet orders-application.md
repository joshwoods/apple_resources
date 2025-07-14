

- Wallet Orders
-  Application 

Object

# Application

The details of an app in the App Store.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
object Application
```

## Properties

`customProductPageIdentifier`

`string`

The identifier for a custom product page. Use when linking to the App on the AppStore.

`launchURL`

`string`

A URL passed into the application at launch.

`storeIdentifier`

`number`

 (Required) 

The ADAM ID (store identifier) of the application.

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

object Return

The details of a return order.

