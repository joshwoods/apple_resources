

- App Store Connect API
-  PrereleaseVersion 

Object

# PrereleaseVersion

The data structure that represents a Prerelease Versions resource.

App Store Connect API 1.0+

``` source
object PrereleaseVersion
```

## Properties

`attributes`

PrereleaseVersion.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

PrereleaseVersion.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `preReleaseVersions`

## Topics

### Objects

object PrereleaseVersion.Attributes

Attributes that describe a Prerelease Versions resource.

object PrereleaseVersion.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object PrereleaseVersionResponse

A response that contains a single Prerelease Versions resource.

object PreReleaseVersionsResponse

A response that contains a list of Pre-Release Version resources.

object PrereleaseVersionWithoutIncludesResponse

object PreReleaseVersionsWithoutIncludesResponse

