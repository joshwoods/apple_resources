

- Enterprise Program API
-  ProfileResponse 

Object

# ProfileResponse

A response that contains a single Profiles resource.

``` source
object ProfileResponse
```

## Properties

`data`

Profile

 (Required) 

The resource data.

`included`

`[*]`

Possible types: BundleId`, `Device`, `Certificate

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

## Attributes 

Possible types:

## See Also

### Objects

object Profile

The data structure that represents a Profiles resource.

object ProfileCreateRequest

The request body you use to create a Profile.

object ProfilesResponse

A response that contains a list of Profiles resources.

object ProfilesWithoutIncludesResponse

