

- App Store Connect API
-  InAppPurchaseImage 

Object

# InAppPurchaseImage

The data structure that represents a in-app purchase image resource.

App Store Connect API 3.6+

``` source
object InAppPurchaseImage
```

## Properties

`attributes`

InAppPurchaseImage.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

InAppPurchaseImage.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `inAppPurchaseImages`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object InAppPurchaseImage.Attributes

Attributes that describe a subscription image resource.

object InAppPurchaseImage.Relationships

The data structure that represents the relationships of a subscription image resource.

## See Also

### Objects

object InAppPurchaseImageCreateRequest

The request body you use to create a in-app purchase purchase image reservation.

object InAppPurchaseImageResponse

A response that contains a single in-app purchase images resource.

object InAppPurchaseImageUpdateRequest

The data structure that represents a in-app purchase image resource.

object InAppPurchaseImagesResponse

A response that contains a list of in-app purchase image resources.

