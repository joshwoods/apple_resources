

- App Store Connect API
-  AppClipHeaderImage 

Object

# AppClipHeaderImage

The data structure that represents the image that appears on the App Clip card of a default App Clip experience.

App Store Connect API 1.6+

``` source
object AppClipHeaderImage
```

## Properties

`attributes`

AppClipHeaderImage.Attributes

The attributes that describe the App Clip Header Images resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies an App Clip Header Images resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

AppClipHeaderImage.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appClipHeaderImages`

## Topics

### Objects

object AppClipHeaderImage.Attributes

The attributes that describe the image that appears on the App Clip card of a default App Clip experience.

object AppClipHeaderImage.Relationships

The relationships of the App Clip Header Images resource you included in the request and those on which you can operate.

## See Also

### Objects

object AppClipHeaderImageResponse

A response that contains a single App Clip Header Images resource.

object AppClipHeaderImageCreateRequest

The request body you use to reserve an image asset that appears on the App Clip card of a default App Clip experience.

object AppClipHeaderImageUpdateRequest

The request body you use to commit the image asset for a default App Clip experience.

