

- App Store Connect API
-  PrereleaseVersionResponse 

Object

# PrereleaseVersionResponse

A response that contains a single Prerelease Versions resource.

App Store Connect API 1.0+

``` source
object PrereleaseVersionResponse
```

## Properties

`data`

PrereleaseVersion

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[*]`

Possible types: Build`, `App

## See Also

### Related Documentation

Read the Prerelease Version of a Build

Get the prerelease version for a specific build.

### Objects

object PrereleaseVersion

The data structure that represents a Prerelease Versions resource.

object PreReleaseVersionsResponse

A response that contains a list of Pre-Release Version resources.

object PrereleaseVersionWithoutIncludesResponse

object PreReleaseVersionsWithoutIncludesResponse

