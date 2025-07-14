

- App Store Connect API
-  AppScreenshot 

Object

# AppScreenshot

The data structure that represent an App Screenshots resource.

App Store Connect API 1.2+

``` source
object AppScreenshot
```

## Properties

`attributes`

AppScreenshot.Attributes

`id`

`string`

 (Required) 

`links`

ResourceLinks

`relationships`

AppScreenshot.Relationships

`type`

`string`

 (Required) 

Value: `appScreenshots`

## Topics

### Objects

object AppScreenshot.Attributes

Attributes that describe an App Screenshots resource.

object AppScreenshot.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object AppScreenshotCreateRequest

The request body you use to create an App Screenshot.

object AppScreenshotUpdateRequest

The request body you use to update an App Screenshot.

object AppScreenshotResponse

A response that contains a single App Screenshots resource.

object AppScreenshotsResponse

A response that contains a list of App Screenshots resources.

object UploadOperation

Upload instructions for assets such as app previews and app screenshots.

