

- App Store Connect API
-  AppStoreVersionLocalizationsResponse 

Object

# AppStoreVersionLocalizationsResponse

A response that contains a list of App Store Version Localization resources.

App Store Connect API 1.2+

``` source
object AppStoreVersionLocalizationsResponse
```

## Properties

`data`

`[`AppStoreVersionLocalization`]`

 (Required) 

`included`

`[*]`

Possible types: AppStoreVersion`, `AppScreenshotSet`, `AppPreviewSet

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object AppStoreVersionLocalization

The data structure that represent an App Store Version Localizations resource.

object AppStoreVersionLocalizationCreateRequest

The request body you use to create an App Store Version Localization.

object AppStoreVersionLocalizationResponse

A response that contains a single App Store Version Localizations resource.

object AppStoreVersionLocalizationUpdateRequest

The request body you use to update an App Store Version Localization

