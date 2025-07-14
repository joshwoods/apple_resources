

- App Store Connect API
-  AppClipDefaultExperiencesResponse 

Object

# AppClipDefaultExperiencesResponse

A response that contains a list of Default App Clip Experiences resources.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperiencesResponse
```

## Properties

`data`

`[`AppClipDefaultExperience`]`

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: AppClip`, `AppStoreVersion`, `AppClipDefaultExperienceLocalization`, `AppClipAppStoreReviewDetail

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## See Also

### Objects

object AppClip

The data structure that represents an App Clips resource.

object AppClipResponse

A response that contains a single App Clips resource.

object AppClipAdvancedExperiencesResponse

A response that contains a list of Advanced App Clip Experiences resources.

