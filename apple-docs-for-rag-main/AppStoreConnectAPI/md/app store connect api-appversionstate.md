

- App Store Connect API
-  AppVersionState 

Type

# AppVersionState

String that represents the state of an app version.

App Store Connect API 3.3+

``` source
string AppVersionState
```

## Possible Values 

`ACCEPTED`  

`DEVELOPER_REJECTED`  

`IN_REVIEW`  

`INVALID_BINARY`  

`METADATA_REJECTED`  

`PENDING_APPLE_RELEASE`  

`PENDING_DEVELOPER_RELEASE`  

`PREPARE_FOR_SUBMISSION`  

`PROCESSING_FOR_DISTRIBUTION`  

`READY_FOR_DISTRIBUTION`  

`READY_FOR_REVIEW`  

`REJECTED`  

`REPLACED_WITH_NEW_VERSION`  

`WAITING_FOR_EXPORT_COMPLIANCE`  

`WAITING_FOR_REVIEW`  

## Mentioned in 

App Store Connect API 3.7 release notes

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

object AppStoreVersionsResponse

A response that contains a list of App Store Version resources.

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

