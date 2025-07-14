

- App Store Connect API
-  AppClipDefaultExperienceLocalizationsResponse 

Object

# AppClipDefaultExperienceLocalizationsResponse

A response that contains a list of Default App Clip Experience Localizations resources.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperienceLocalizationsResponse
```

## Properties

`data`

`[`AppClipDefaultExperienceLocalization`]`

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: AppClipDefaultExperience`, `AppClipHeaderImage

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## See Also

### Objects

object AppClipDefaultExperienceLocalization

The data structure that represents a Default App Clip Experience Localizations resource.

object AppClipDefaultExperienceLocalizationResponse

A response that contains a single Default App Clip Experience Localizations resource.

object AppClipDefaultExperienceLocalizationCreateRequest

The request body you use to create a Default App Clip Experience Localization.

object AppClipDefaultExperienceLocalizationUpdateRequest

The request body you use to update a Default App Clip Experiences resource.

