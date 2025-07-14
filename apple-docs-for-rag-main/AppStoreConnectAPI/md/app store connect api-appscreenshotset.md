

- App Store Connect API
-  AppScreenshotSet 

Object

# AppScreenshotSet

The data structure that represent an app screenshot set resource.

App Store Connect API 1.2+

``` source
object AppScreenshotSet
```

## Properties

`attributes`

AppScreenshotSet.Attributes

`id`

`string`

 (Required) 

`links`

ResourceLinks

`relationships`

AppScreenshotSet.Relationships

`type`

`string`

 (Required) 

Value: `appScreenshotSets`

## Topics

### Objects

object AppScreenshotSet.Attributes

Attributes that describe an App Screenshot Sets resource.

object AppScreenshotSet.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and Data Types

object AppScreenshotSetCreateRequest

The request body you use to create an app screenshot set.

object AppScreenshotSetResponse

A response that contains a single app screenshot set resource.

object AppScreenshotSetsResponse

A response that contains a list of app screenshot set resources.

object AppScreenshotSetAppScreenshotsLinkagesRequest

A request body you use to reorder the screenshots in a screenshot set.

object AppScreenshotSetAppScreenshotsLinkagesResponse

A response body that contains a list of related resource IDs.

type ScreenshotDisplayType

A string that represents the display type of an app screenshot.

