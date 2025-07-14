

- App Store Connect API
-  BuildsResponse 

Object

# BuildsResponse

A response that contains a list of Builds resources.

App Store Connect API 1.0+

``` source
object BuildsResponse
```

## Properties

`data`

`[`Build`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

`included`

`[*]`

Possible types: PrereleaseVersion`, `BetaTester`, `BetaGroup`, `BetaBuildLocalization`, `AppEncryptionDeclaration`, `BetaAppReviewSubmission`, `App`, `BuildBetaDetail`, `AppStoreVersion`, `BuildIcon`, `BuildBundle

## See Also

### Related Documentation

List All Builds for a Beta Group

Get a list of builds associated with a specific beta group.

### Objects

object Build

The data structure that represents a Builds resource.

object BuildResponse

A response that contains a single Builds resource.

object BuildWithoutIncludesResponse

object BuildsWithoutIncludesResponse

object BuildUpdateRequest

The request body you use to update a Build.

object BuildAppEncryptionDeclarationLinkageRequest

The request body you use to attach an app encryption declaration to a build.

object BuildAppEncryptionDeclarationLinkageResponse

A response body that contains the ID of a single related resource.

object BuildIndividualTestersLinkagesRequest

A request body you use to add or remove a build from multiple beta groups.

object BuildIndividualTestersLinkagesResponse

A response body that contains a list of related resource IDs.

object BuildBetaGroupsLinkagesRequest

A request body you use to add or remove beta groups from a build.

object ImageAsset

An image asset, including its height, width, and template URL.

object BetaBuildUsagesV1MetricResponse

A response that contains one or more beta build metric resources.

