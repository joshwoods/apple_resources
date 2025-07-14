

- App Store Connect API
-  AppClip 

Object

# AppClip

The data structure that represents an App Clips resource.

App Store Connect API 1.6+

``` source
object AppClip
```

## Properties

`attributes`

AppClip.Attributes

The attributes that describe the App Clips resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies an App Clips resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

AppClip.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appClips`

## Topics

### Objects

object AppClip.Attributes

The attributes that describe an App Clips resource.

object AppClip.Relationships

The relationships of the App Clips resource you included in the request and those on which you can operate.

## See Also

### Objects

object AppClipResponse

A response that contains a single App Clips resource.

object AppClipDefaultExperiencesResponse

A response that contains a list of Default App Clip Experiences resources.

object AppClipAdvancedExperiencesResponse

A response that contains a list of Advanced App Clip Experiences resources.

