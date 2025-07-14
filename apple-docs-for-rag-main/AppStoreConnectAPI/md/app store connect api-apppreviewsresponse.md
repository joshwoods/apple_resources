

- App Store Connect API
-  AppPreviewsResponse 

Object

# AppPreviewsResponse

A response that contains a list of App Preview resources.

App Store Connect API 1.2+

``` source
object AppPreviewsResponse
```

## Properties

`data`

`[`AppPreview`]`

 (Required) 

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

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

object AppPreviewResponse

A response that contains a single App Previews resource.

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

