

- App Store Connect API
-  CiProductResponse 

Object

# CiProductResponse

A response that contains a single Products resource.

App Store Connect API 1.5+

``` source
object CiProductResponse
```

## Properties

`data`

CiProduct

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: App`, `BundleId`, `ScmRepository

`links`

DocumentLinks

 (Required) 

The navigational links that include the self-link.

## See Also

### Objects

object CiProduct

The data structure that represents a Products resource.

object CiProductsResponse

A response that contains a list of Products resources.

