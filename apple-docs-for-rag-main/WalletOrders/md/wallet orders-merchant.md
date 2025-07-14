

- Wallet Orders
-  Merchant 

Object

# Merchant

The merchant associated with the order.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
object Merchant
```

## Properties

`address`

Address

The contact address of the merchant.

`businessChatURL`

`uri`

An Apple Messages for Business URL the customer uses to contact the merchant. For more information, see Starting a Message from a URL.

`contactURL`

`uri`

The URL where the customer can contact the merchant.

`displayName`

`string`

 (Required) 

The localized display name of the merchant.

`emailAddress`

`string`

The email address where the customer can contact the merchant.

`logo`

`string`

The name for an image representing the merchant’s logo.

`merchantIdentifier`

`string`

 (Required) 

The Apple Merchant Identifier for this merchant, generated at developer.apple.com.

`phoneNumber`

`string`

The telephone number where the customer can contact the merchant.

`url`

`uri`

 (Required) 

The URL for the merchant’s website or landing page.

## Attributes 

Possible types:

## See Also

### Supporting objects

object Customer

The details of the order’s customer.

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

object Return

The details of a return order.

