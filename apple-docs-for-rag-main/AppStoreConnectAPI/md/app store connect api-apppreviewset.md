

- App Store Connect API
-  AppPreviewSet 

Object

# AppPreviewSet

The data structure that represent an App Preview Sets resource.

App Store Connect API 1.2+

``` source
object AppPreviewSet
```

## Properties

`attributes`

AppPreviewSet.Attributes

`id`

`string`

 (Required) 

`links`

ResourceLinks

`relationships`

AppPreviewSet.Relationships

`type`

`string`

 (Required) 

Value: `appPreviewSets`

## Topics

### Objects

object AppPreviewSet.Attributes

Attributes that describe an App Preview Sets resource.

object AppPreviewSet.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object AppPreviewSetCreateRequest

The request body you use to create an App Preview Set.

object AppPreviewSetResponse

A response that contains a single App Preview Sets resource.

object AppPreviewSetsResponse

A response that contains a list of App Preview Set resources.

object AppPreviewSetAppPreviewsLinkagesRequest

A request body you use to reorder the app previews in a preview set.

object AppPreviewSetAppPreviewsLinkagesResponse

A response body that contains a list of related resource IDs.

