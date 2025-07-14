

- App Store Connect API
-  AppPreview 

Object

# AppPreview

The data structure that represent an App Previews resource.

App Store Connect API 1.2+

``` source
object AppPreview
```

## Properties

`attributes`

AppPreview.Attributes

`id`

`string`

 (Required) 

`links`

ResourceLinks

`relationships`

AppPreview.Relationships

`type`

`string`

 (Required) 

Value: `appPreviews`

## Topics

### Objects

object AppPreview.Attributes

Attributes that describe an App Previews resource.

object AppPreview.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and Data Types

object AppPreviewCreateRequest

The request body you use to create an App Preview.

object AppPreviewUpdateRequest

The request body you use to update an App Preview.

object AppPreviewResponse

A response that contains a single App Previews resource.

object AppPreviewsResponse

A response that contains a list of App Preview resources.

object UploadOperation

Upload instructions for assets such as app previews and app screenshots.

type PreviewType

String that represents the display type of an app preview.

object PreviewFrameImage

The properties that describe a preview frame image for an app preview or app event video.

object AppMediaVideoState

The properties that describe the state of an app preview or app event video.

object AppMediaPreviewFrameImageState

The properties that describe the state of a preview frame image for an app preveiew or app event video.

