

- App Store Connect API
-  AppScreenshotSetResponse 

Object

# AppScreenshotSetResponse

A response that contains a single app screenshot set resource.

App Store Connect API 1.2+

``` source
object AppScreenshotSetResponse
```

## Properties

`data`

AppScreenshotSet

 (Required) 

`included`

`[*]`

Possible types: AppStoreVersionLocalization`, `AppCustomProductPageLocalization`, `AppStoreVersionExperimentTreatmentLocalization`, `AppScreenshot

`links`

DocumentLinks

 (Required) 

## See Also

### Objects and Data Types

object AppScreenshotSet

The data structure that represent an app screenshot set resource.

object AppScreenshotSetCreateRequest

The request body you use to create an app screenshot set.

object AppScreenshotSetsResponse

A response that contains a list of app screenshot set resources.

object AppScreenshotSetAppScreenshotsLinkagesRequest

A request body you use to reorder the screenshots in a screenshot set.

object AppScreenshotSetAppScreenshotsLinkagesResponse

A response body that contains a list of related resource IDs.

type ScreenshotDisplayType

A string that represents the display type of an app screenshot.

