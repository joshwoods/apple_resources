

- App Store Connect API
-  ProfilesResponse 

Object

# ProfilesResponse

A response that contains a list of Profiles resources.

App Store Connect API 1.1+

``` source
object ProfilesResponse
```

## Properties

`data`

`[`Profile`]`

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

Possible types: BundleId`, `Device`, `Certificate

## See Also

### Related Documentation

List and Download Profiles

Find and list provisioning profiles and download their data.

### Objects

object Profile

The data structure that represents a Profiles resource.

object ProfileCreateRequest

The request body you use to create a Profile.

object ProfileResponse

A response that contains a single Profiles resource.

object ProfilesWithoutIncludesResponse

