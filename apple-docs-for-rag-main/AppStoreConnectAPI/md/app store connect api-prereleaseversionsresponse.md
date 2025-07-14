

- App Store Connect API
-  PreReleaseVersionsResponse 

Object

# PreReleaseVersionsResponse

A response that contains a list of Pre-Release Version resources.

App Store Connect API 1.0+

``` source
object PreReleaseVersionsResponse
```

## Properties

`data`

`[`PrereleaseVersion`]`

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

Possible types: Build`, `App

## See Also

### Related Documentation

List Prerelease Versions

Get a list of prerelease versions for all apps.

### Objects

object PrereleaseVersion

The data structure that represents a Prerelease Versions resource.

object PrereleaseVersionResponse

A response that contains a single Prerelease Versions resource.

object PrereleaseVersionWithoutIncludesResponse

object PreReleaseVersionsWithoutIncludesResponse

