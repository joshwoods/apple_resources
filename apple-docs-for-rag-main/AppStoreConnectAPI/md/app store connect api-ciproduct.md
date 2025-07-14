

- App Store Connect API
-  CiProduct 

Object

# CiProduct

The data structure that represents a Products resource.

App Store Connect API 1.5+

``` source
object CiProduct
```

## Properties

`attributes`

CiProduct.Attributes

The attributes that describe the Products resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Products resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

CiProduct.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `ciProducts`

## Topics

### Objects

object CiProduct.Attributes

The attributes that describe a Products resource.

object CiProduct.Relationships

The relationships of the Products resource you included in the request and those on which you can operate.

## See Also

### Objects

object CiProductResponse

A response that contains a single Products resource.

object CiProductsResponse

A response that contains a list of Products resources.

