

- Advanced Commerce API
-  SubscriptionModifyInAppRequest 

Object

# SubscriptionModifyInAppRequest

The request data your app provides to make changes to an auto-renewable subscription.

Advanced Commerce API 1.0+

``` source
object SubscriptionModifyInAppRequest
```

## Properties

`addItems`

`[`SubscriptionModifyAddItem`]`

`changeItems`

`[`SubscriptionModifyChangeItem`]`

`currency`

currency

`descriptors`

SubscriptionModifyDescriptors

`operation`

`string`

 (Required) 

Value: `MODIFY_SUBSCRIPTION`

`periodChange`

SubscriptionModifyPeriodChange

`removeItems`

`[`SubscriptionModifyRemoveItem`]`

`requestInfo`

RequestInfo

 (Required) 

`retainBillingCycle`

retainBillingCycle

 (Required) 

`storefront`

storefront

`taxCode`

taxCode

`transactionId`

transactionId

 (Required) 

`version`

version

 (Required) 

## See Also

### Subscription modification in the app

object SubscriptionModifyAddItem

The data your app provides to add items when it makes changes to an auto-renewable subscription.

object SubscriptionModifyChangeItem

The data your app provides to change an item of an auto-renewable subscription.

object SubscriptionModifyRemoveItem

The data your app provides to remove an item from an auto-renewable subscription.

object SubscriptionModifyPeriodChange

The data your app provides to change the period of an auto-renewable subscription.

