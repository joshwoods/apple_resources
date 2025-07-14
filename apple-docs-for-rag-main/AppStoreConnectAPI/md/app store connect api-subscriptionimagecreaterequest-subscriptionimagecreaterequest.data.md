

- App Store Connect API
- SubscriptionImageCreateRequest
-  SubscriptionImageCreateRequest.Data 

Object

# SubscriptionImageCreateRequest.Data

The request body you use to create a subscription purchase image reservation.

App Store Connect API 3.6+

``` source
object SubscriptionImageCreateRequest.Data
```

## Properties

`attributes`

SubscriptionImageCreateRequest.Data.Attributes

 (Required) 

The resource’s attributes.

`relationships`

SubscriptionImageCreateRequest.Data.Relationships

 (Required) 

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `subscriptionImages`

## Topics

### Objects

object SubscriptionImageCreateRequest.Data.Attributes

Attributes that describe a subscription purchase image request resource.

object SubscriptionImageCreateRequest.Data.Relationships

The relationships you included in the request and those on which you can operate.

