

- Wallet Orders
-  OrderProvider 

Object

# OrderProvider

Information about the platform providing the order data.

iOS 17.4+iPadOS 17.4+macOS 14.4+

``` source
object OrderProvider
```

## Properties

`displayName`

`string`

 (Required) 

The localized display name of the order provider platform.

`trackingLogoNameDarkColorScheme`

`string`

 (Required) 

The name of the logo image for the order provider that’s intended for the dark color scheme. When the shipping fulfilment has a `trackingURL`, it uses this image.

`trackingLogoNameLightColorScheme`

`string`

 (Required) 

The name of the logo image for the order provider that’s intended for the light color scheme. When the shipping fulfilment has a `trackingURL`, it uses this image.

`url`

`uri`

 (Required) 

The URL of the order provder platform.

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

