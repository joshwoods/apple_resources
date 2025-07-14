

- Enterprise Program API
-  ProfilesResponse 

Object

# ProfilesResponse

A response that contains a list of Profiles resources.

``` source
object ProfilesResponse
```

## Properties

`data`

`[`Profile`]`

 (Required) 

The resource data.

`included`

`[*]`

Possible types: BundleId`, `Device`, `Certificate

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

## Attributes 

Possible types:

## See Also

### Objects

object Profile

The data structure that represents a Profiles resource.

object ProfileCreateRequest

The request body you use to create a Profile.

object ProfileResponse

A response that contains a single Profiles resource.

object ProfilesWithoutIncludesResponse

