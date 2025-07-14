

- Advanced Commerce API
-  SubscriptionCreateRequest 

Object

# SubscriptionCreateRequest

The metadata your app provides when a customer purchases an auto-renewable subscription.

Advanced Commerce API 1.0+

``` source
object SubscriptionCreateRequest
```

## Properties

`currency`

currency

 (Required) 

`descriptors`

Descriptors

 (Required) 

`items`

`[`SubscriptionCreateItem`]`

 (Required) 

`operation`

`string`

 (Required) 

Value: `CREATE_SUBSCRIPTION`

`period`

period

 (Required) 

`previousTransactionId`

transactionId

`requestInfo`

RequestInfo

 (Required) 

`storefront`

storefront

`taxCode`

taxCode

 (Required) 

`version`

version

 (Required) 

## Mentioned in 

Creating SKUs for your In-App Purchases

## See Also

### Subscription creation in the app

object SubscriptionCreateItem

The data that describes a subscription item.

