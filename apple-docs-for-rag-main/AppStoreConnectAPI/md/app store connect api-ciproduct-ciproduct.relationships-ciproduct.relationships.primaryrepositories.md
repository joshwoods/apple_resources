

- App Store Connect API
- CiProduct
- CiProduct.Relationships
-  CiProduct.Relationships.PrimaryRepositories 

Object

# CiProduct.Relationships.PrimaryRepositories

The data, links, and paging information that describe the relationship between the Products resource and the Repositories resource that represents the primary repository.

App Store Connect API 1.5+

``` source
object CiProduct.Relationships.PrimaryRepositories
```

## Properties

`data`

`[`CiProduct.Relationships.PrimaryRepositories.Data`]`

The ID and type of the related Repositories resource that represents the primary repository.

`links`

RelationshipLinks

The navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## Topics

### Objects

object CiProduct.Relationships.PrimaryRepositories.Data

The type and ID of a related Repositories resource that represents the product’s primary repositories.

## See Also

### Objects

object CiProduct.Relationships.App

The data and links that describe the relationship between the Products and Apps resources.

object CiProduct.Relationships.BundleId

The data and links that describe the relationship between the Products and the Bundle IDs resources.

