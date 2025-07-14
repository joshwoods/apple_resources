

- App Store Connect API
-  AppStoreVersion 

Object

# AppStoreVersion

The data structure that represent an App Store Versions resource.

App Store Connect API 1.2+

``` source
object AppStoreVersion
```

## Properties

`attributes`

AppStoreVersion.Attributes

`id`

`string`

 (Required) 

`relationships`

AppStoreVersion.Relationships

`type`

`string`

 (Required) 

Value: `appStoreVersions`

`links`

ResourceLinks

## Topics

### Objects

object AppStoreVersion.Attributes

Attributes that describe an App Store Versions resource.

object AppStoreVersion.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects and Data Types

object AppStoreVersionUpdateRequest

The request body you use to update an App Store Version.

object AgeRatingDeclaration

The data structure that represents an Age Rating Declarations resource.

object AgeRatingDeclarationWithoutIncludesResponse

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

type AppVersionState

String that represents the state of an app version.

