

- Wallet Orders
-  PickupFulfillment 

Object

# PickupFulfillment

The details of a pickup order.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
object PickupFulfillment
```

## Properties

`address`

Address

The address for the order pickup.

`barcode`

Barcode

The barcode the customer shows at pickup.

`displayName`

`string`

 (Required) 

The localized name of the pickup location.

`fulfillmentIdentifier`

`string`

 (Required) 

An opaque value that uniquely identifies this fulfillment in the order. This isn’t displayed to the user and only for determining changes and user notifications.

`fulfillmentType`

`string`

 (Required) 

The type of fulfillment, which is `pickup`.

Value: `pickup`

`lineItems`

`[`LineItem`]`

The items for the customer to pick up, displayed in the order provided.

`location`

Location

The latitude and longitude of the pickup location. Use this when you require greater precision than address alone (for example, for accurate indoor mapping display).

`notes`

`string`

Localized instructions for the pickup.

`pickedUpAt`

`date-time`

The date and time when the customer picked up the order, in RFC 3339 format.

`pickupAt`

`date-time`

The date and time when the pickup window starts, in RFC 3339 format.

`pickupWindowDuration`

`duration`

The duration for which the pickup window is open, in ISO 8601-1 duration format.

`status`

`string`

 (Required) 

The status of the fulfillment.

Possible Values: `open, processing, readyForPickup, pickedUp, issue, cancelled`

`statusDescription`

`string`

A localized message describing the fulfillment status.

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

object Return

The details of a return order.

