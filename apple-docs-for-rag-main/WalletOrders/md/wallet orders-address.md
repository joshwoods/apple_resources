

- Wallet Orders
-  Address 

Object

# Address

The physical address for an order.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
object Address
```

## Properties

`addressLines`

`[string]`

The street portion of the address.

`administrativeArea`

`string`

The state or administrative area of the address.

`countryCode`

`string`

The country of the address, in ISO-3166 two-letter format.

Minimum length: `2`

Maximum length: `2`

`locality`

`string`

The city of the address.

`postalCode`

`string`

The ZIP or postal code, where applicable, of the address.

`subAdministrativeArea`

`string`

The subadministrative area (such as county or other region) of the address.

`subLocality`

`string`

Additional information associated with the location, such as a district or neighborhood.

## Attributes 

Possible types:

## See Also

### Supporting objects

object Customer

The details of the order’s customer.

object Merchant

The merchant associated with the order.

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

object Return

The details of a return order.

