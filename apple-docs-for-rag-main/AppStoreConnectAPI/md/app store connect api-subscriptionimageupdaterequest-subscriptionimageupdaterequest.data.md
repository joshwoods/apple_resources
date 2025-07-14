

- App Store Connect API
- SubscriptionImageUpdateRequest
-  SubscriptionImageUpdateRequest.Data 

Object

# SubscriptionImageUpdateRequest.Data

The request body you use to update a subscription purchase image reservation.

App Store Connect API 3.6+

``` source
object SubscriptionImageUpdateRequest.Data
```

## Properties

`attributes`

SubscriptionImageUpdateRequest.Data.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `subscriptionImages` resource ID from the List subscription images response.

`type`

`string`

 (Required) 

The resource type.

Value: `subscriptionImages`

## Topics

### Objects

object SubscriptionImageUpdateRequest.Data.Attributes

Attributes that describe a subscription image request resource.

