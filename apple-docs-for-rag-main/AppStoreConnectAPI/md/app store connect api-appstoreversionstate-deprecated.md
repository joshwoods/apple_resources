

- App Store Connect API
-  AppStoreVersionState Deprecated

Type

# AppStoreVersionState

String that represents the state of an app version in the App Store.

App Store Connect API 1.2–3.7Deprecated

``` source
string AppStoreVersionState
```

Deprecated

Use \`AppVersionState\`\` instead.

## Possible Values 

`ACCEPTED`  

`DEVELOPER_REMOVED_FROM_SALE`  

`DEVELOPER_REJECTED`  

`IN_REVIEW`  

`INVALID_BINARY`  

`METADATA_REJECTED`  

`PENDING_APPLE_RELEASE`  

`PENDING_CONTRACT`  

`PENDING_DEVELOPER_RELEASE`  

`PREPARE_FOR_SUBMISSION`  

`PREORDER_READY_FOR_SALE`  

`PROCESSING_FOR_APP_STORE`  

`READY_FOR_REVIEW`  

`READY_FOR_SALE`  

`REJECTED`  

`REMOVED_FROM_SALE`  

`WAITING_FOR_EXPORT_COMPLIANCE`  

`WAITING_FOR_REVIEW`  

`REPLACED_WITH_NEW_VERSION`  

`NOT_APPLICABLE`  

## Discussion

- PossibleValues

  - DEVELOPER_REMOVED_FROM_SALE

  - DEVELOPER_REJECTED

  - IN_REVIEW

  - INVALID_BINARY

  - METADATA_REJECTED

  - PENDING_APPLE_RELEASE

  - PENDING_CONTRACT

  - PENDING_DEVELOPER_RELEASE

  - PREPARE_FOR_SUBMISSION

  - PREORDER_READY_FOR_SALE

  - PROCESSING_FOR_APP_STORE

  - READY_FOR_SALE

  - REJECTED

  - REMOVED_FROM_SALE

  - WAITING_FOR_EXPORT_COMPLIANCE

  - WAITING_FOR_REVIEW

  - REPLACED_WITH_NEW_VERSION

  - ACCEPTED

  - READY_FOR_REVIEW

  - NOT_APPLICABLE

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

type AppVersionState

String that represents the state of an app version.

