

- App Store Connect API
-  AppClipAdvancedExperiencesResponse 

Object

# AppClipAdvancedExperiencesResponse

A response that contains a list of Advanced App Clip Experiences resources.

App Store Connect API 1.6+

``` source
object AppClipAdvancedExperiencesResponse
```

## Properties

`data`

`[`AppClipAdvancedExperience`]`

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: AppClip`, `AppClipAdvancedExperienceImage`, `AppClipAdvancedExperienceLocalization

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

object AppClipDefaultExperiencesResponse

A response that contains a list of Default App Clip Experiences resources.

