

- App Store Connect API
-  AppScreenshotsResponse 

Object

# AppScreenshotsResponse

A response that contains a list of App Screenshots resources.

App Store Connect API 1.2+

``` source
object AppScreenshotsResponse
```

## Properties

`data`

`[`AppScreenshot`]`

 (Required) 

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

`included`

`[`AppScreenshotSet`]`

## See Also

### Objects

object AppScreenshot

The data structure that represent an App Screenshots resource.

object AppScreenshotCreateRequest

The request body you use to create an App Screenshot.

object AppScreenshotUpdateRequest

The request body you use to update an App Screenshot.

object AppScreenshotResponse

A response that contains a single App Screenshots resource.

object UploadOperation

Upload instructions for assets such as app previews and app screenshots.

