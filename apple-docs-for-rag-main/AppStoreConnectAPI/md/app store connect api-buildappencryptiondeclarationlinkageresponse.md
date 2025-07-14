

- App Store Connect API
-  BuildAppEncryptionDeclarationLinkageResponse 

Object

# BuildAppEncryptionDeclarationLinkageResponse

A response body that contains the ID of a single related resource.

App Store Connect API 1.0+

``` source
object BuildAppEncryptionDeclarationLinkageResponse
```

## Properties

`data`

BuildAppEncryptionDeclarationLinkageResponse.Data

 (Required) 

The object types and IDs of the related resources.

`links`

DocumentLinks

 (Required) 

Navigational links including the self-link and links to the related data.

## Topics

### Objects

object BuildAppEncryptionDeclarationLinkageResponse.Data

The data element of the response body.

## See Also

### Related Documentation

Get the App Encryption Declaration ID for a Build

Get the beta app encryption declaration resource ID associated with a build.

### Objects

object Build

The data structure that represents a Builds resource.

object BuildResponse

A response that contains a single Builds resource.

object BuildWithoutIncludesResponse

object BuildsResponse

A response that contains a list of Builds resources.

object BuildsWithoutIncludesResponse

object BuildUpdateRequest

The request body you use to update a Build.

object BuildAppEncryptionDeclarationLinkageRequest

The request body you use to attach an app encryption declaration to a build.

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

