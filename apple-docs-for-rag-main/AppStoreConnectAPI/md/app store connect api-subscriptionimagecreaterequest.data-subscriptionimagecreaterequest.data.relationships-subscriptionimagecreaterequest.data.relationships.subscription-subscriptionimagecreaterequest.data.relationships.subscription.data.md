

- App Store Connect API
- SubscriptionImageCreateRequest
- 
  - SubscriptionImageCreateRequest
- SubscriptionImageCreateRequest.Data
- SubscriptionImageCreateRequest.Data.Relationships
- SubscriptionImageCreateRequest.Data.Relationships.Subscription
-  SubscriptionImageCreateRequest.Data.Relationships.Subscription.Data 

Object

# SubscriptionImageCreateRequest.Data.Relationships.Subscription.Data

The data structure that represents the subscription for a subscription image create request resource.

App Store Connect API 3.6+

``` source
object SubscriptionImageCreateRequest.Data.Relationships.Subscription.Data
```

## Properties

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `subscriptions` resource ID from the List All Subscriptions for a Subscription Group response.

`type`

`string`

 (Required) 

Value: `subscriptions`

