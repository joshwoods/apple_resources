

- App Store Connect API
-  ProfileResponse 

Object

# ProfileResponse

A response that contains a single Profiles resource.

App Store Connect API 1.1+

``` source
object ProfileResponse
```

## Properties

`data`

Profile

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[*]`

Possible types: BundleId`, `Device`, `Certificate

## See Also

### Related Documentation

Create a Profile

Create a new provisioning profile.

### Objects

object Profile

The data structure that represents a Profiles resource.

object ProfileCreateRequest

The request body you use to create a Profile.

object ProfilesResponse

A response that contains a list of Profiles resources.

object ProfilesWithoutIncludesResponse

