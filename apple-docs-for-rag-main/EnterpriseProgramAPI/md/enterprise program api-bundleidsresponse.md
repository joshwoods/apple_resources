

- Enterprise Program API
-  BundleIdsResponse 

Object

# BundleIdsResponse

A response that contains a list of Bundle ID resources.

``` source
object BundleIdsResponse
```

## Properties

`data`

`[`BundleId`]`

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

The requested relationship data.

Possible types: Profile`, `BundleIdCapability

## Attributes 

Possible types:

## See Also

### Objects and Types

object BundleId

The data structure that represents a Bundle IDs resource.

type BundleIdPlatform

Strings that represent the operating system intended for the bundle.

object BundleIdCreateRequest

The request body you use to create a Bundle ID.

object BundleIdUpdateRequest

The request body you use to update a Bundle ID.

object BundleIdResponse

A response that contains a single Bundle IDs resource.

object BundleIdWithoutIncludesResponse

A response that contains a single Bundle IDs resource without includes.

