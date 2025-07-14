

- Wallet Orders
-  Location 

Object

# Location

A geographic location.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
object Location
```

## Properties

`altitude`

`number`

The altitude above mean sea level, measured in meters.

`latitude`

`number`

 (Required) 

The latitude of the location.

Minimum: `-90`

Maximum: `90`

`longitude`

`number`

 (Required) 

The longitude of the location.

Minimum: `-180`

Maximum: `180`

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

