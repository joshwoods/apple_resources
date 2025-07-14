

- Wallet Orders
-  ReturnInfo 

Object

# ReturnInfo

The information related to a partial or full return.

iOS 17.2+iPadOS 17.2+macOS 14.2+

``` source
object ReturnInfo
```

## Properties

`returnPolicyURL`

`uri`

 (Required) 

The URL where the customer can see the order return policy.

`displayCountdown`

`boolean`

A Boolean value that indicates whether to display the return countdown until `returnDeadline` in the user interface. Use `true` if all of the items in the order are returnable until the `returnDeadline`.

Default: `false`

`returnDeadline`

`date-time`

The date where the products can be partially or fully returned. The merchant can provide updates to an order that has a completed status until this date.

Use `ISO 8601` format.

`returnManagementURL`

`uri`

The URL where the customer can initiate a return.

`returnPolicyDescription`

`string`

A short description of the return policy. The merchant can include the common return window duration here.

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

