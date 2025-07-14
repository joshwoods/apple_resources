

- App Store Connect API
-  AppClipDefaultExperienceResponse 

Object

# AppClipDefaultExperienceResponse

A response that contains a single Default App Clip Experiences resource.

App Store Connect API 1.6+

``` source
object AppClipDefaultExperienceResponse
```

## Properties

`data`

AppClipDefaultExperience

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: AppClip`, `AppStoreVersion`, `AppClipDefaultExperienceLocalization`, `AppClipAppStoreReviewDetail

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## See Also

### Objects and Types

object AppClipDefaultExperience

The data structure that represents a Default App Clip Experiences resource.

object AppClipDefaultExperienceCreateRequest

The request body you use to create a default App Clip experience.

object AppClipDefaultExperienceUpdateRequest

The request body you use to update a default App Clip experience.

object AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageRequest

The request body you use to relate a released App Store version with a default App Clip experience.

object AppClipDefaultExperienceReleaseWithAppStoreVersionLinkageResponse

A response that contains the ID of a single related App Store Versions resource.

type AppClipAction

A string that represents the call- termto- termaction verb on the App Clip card.

