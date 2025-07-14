

- App Store Connect API
-  SubscriptionImage 

Object

# SubscriptionImage

The data structure that represents a subscription image resource.

App Store Connect API 3.6+

``` source
object SubscriptionImage
```

## Properties

`attributes`

SubscriptionImage.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

SubscriptionImage.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `subscriptionImages`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object SubscriptionImage.Attributes

Attributes that describe a subscription image resource.

object SubscriptionImage.Relationships

The data structure that represents the relationships of a subscription image resource.

## See Also

### Objects

object SubscriptionImageCreateRequest

The request body you use to create a subscription purchase image reservation.

object SubscriptionImageResponse

A response that contains a single subscription images resource.

object SubscriptionImagesResponse

A response that contains a list of subscription image resources.

object SubscriptionImageUpdateRequest

The data structure that represents a subscription image update request resource.

