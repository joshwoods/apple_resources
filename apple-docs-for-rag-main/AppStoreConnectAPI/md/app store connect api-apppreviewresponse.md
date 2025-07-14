

- App Store Connect API
-  AppPreviewResponse 

Object

# AppPreviewResponse

A response that contains a single App Previews resource.

App Store Connect API 1.2+

``` source
object AppPreviewResponse
```

## Properties

`data`

AppPreview

 (Required) 

`links`

DocumentLinks

 (Required) 

`included`

`[`AppPreviewSet`]`

## See Also

### Objects and Data Types

object AppPreview

The data structure that represent an App Previews resource.

object AppPreviewCreateRequest

The request body you use to create an App Preview.

object AppPreviewUpdateRequest

The request body you use to update an App Preview.

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

