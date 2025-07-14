

- Advanced Commerce API
-  Offer 

Object

# Offer

A discount offer for an auto-renewable subscription.

Advanced Commerce API 1.0+

``` source
object Offer
```

## Properties

`period`

`string`

 (Required) 

The period of the offer.

Possible Values: `P3D, P1W, P2W, P1M, P2M, P3M, P6M, P9M, P1Y`

`periodCount`

`int32`

 (Required) 

The number of periods the offer is active.

Minimum: `1`

Maximum: `12`

`price`

price

 (Required) 

The offer price, in milliunits.

`reason`

`string`

 (Required) 

The reason for the offer.

Possible Values: `ACQUISITION, WIN_BACK, RETENTION`

## See Also

### Objects

object Descriptors

The display name and description of a subscription product.

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

