

- Advanced Commerce API
-  Descriptors 

Object

# Descriptors

The display name and description of a subscription product.

Advanced Commerce API 1.0+

``` source
object Descriptors
```

## Properties

`description`

description

 (Required) 

A string that contains a description of the product. This string is not displayed to customers.

Maximum length: `45`

`displayName`

displayName

 (Required) 

A string that contains the name of the product, suitable for display to customers.

Maximum length: `30`

## See Also

### Objects

object Offer

A discount offer for an auto-renewable subscription.

object RequestInfo

The metadata to include in server requests.

object SubscriptionModifyAddItem

The data your app provides to add items when it makes changes to an auto-renewable subscription.

object SubscriptionModifyChangeItem

The data your app provides to change an item of an auto-renewable subscription.

object SubscriptionModifyDescriptors

The data your app provides to change the description and display name of an auto-renewable subscription.

object SubscriptionModifyPeriodChange

The data your app provides to change the period of an auto-renewable subscription.

object SubscriptionModifyRemoveItem

The data your app provides to remove an item from an auto-renewable subscription.

object SubscriptionPriceChangeItem

The data your app provides to change a subscription price.

