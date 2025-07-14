

- App Store Connect API
-  AppStoreVersionsResponse 

Object

# AppStoreVersionsResponse

A response that contains a list of App Store Version resources.

App Store Connect API 1.2+

``` source
object AppStoreVersionsResponse
```

## Properties

`data`

`[`AppStoreVersion`]`

 (Required) 

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

`included`

`[*]`

Possible types: App`, `AgeRatingDeclaration`, `AppStoreVersionLocalization`, `Build`, `AppStoreVersionPhasedRelease`, `GameCenterAppVersion`, `RoutingAppCoverage`, `AppStoreReviewDetail`, `AppStoreVersionSubmission`, `AppClipDefaultExperience`, `AppStoreVersionExperiment`, `AppStoreVersionExperimentV2`, `AlternativeDistributionPackage

## See Also

### Objects and Data Types

object AppStoreVersionUpdateRequest

The request body you use to update an App Store Version.

object AgeRatingDeclaration

The data structure that represents an Age Rating Declarations resource.

object AgeRatingDeclarationWithoutIncludesResponse

object AppStoreVersion

The data structure that represent an App Store Versions resource.

object AppStoreVersionResponse

A response that contains a single App Store Versions resource.

object AppStoreVersionCreateRequest

The request body you use to create an App Store Version.

object AppStoreVersionBuildLinkageRequest

The request body you use to attach a build to an App Store version.

object AppStoreVersionBuildLinkageResponse

A response body that contains the ID of a single related resource.

object AppStoreVersionAppClipDefaultExperienceLinkageRequest

The request body you use to attach a default App Clip experience to an App Store version.

object AppStoreVersionAppClipDefaultExperienceLinkageResponse

A response that contains the ID of a single related Default App Clip Experiences resource.

type AppStoreVersionState

String that represents the state of an app version in the App Store.

Deprecated

type AppVersionState

String that represents the state of an app version.

