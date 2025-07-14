

- App Store Connect API
-  CiProductsResponse 

Object

# CiProductsResponse

A response that contains a list of Products resources.

App Store Connect API 1.5+

``` source
object CiProductsResponse
```

## Properties

`data`

`[`CiProduct`]`

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: App`, `BundleId`, `ScmRepository

`links`

PagedDocumentLinks

 (Required) 

The navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## See Also

### Objects

object CiProduct

The data structure that represents a Products resource.

object CiProductResponse

A response that contains a single Products resource.

