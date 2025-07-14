

- App Store Connect API
- CiProduct
-  CiProduct.Relationships 

Object

# CiProduct.Relationships

The relationships of the Products resource you included in the request and those on which you can operate.

App Store Connect API 1.5+

``` source
object CiProduct.Relationships
```

## Properties

`app`

CiProduct.Relationships.App

The related Apps resource.

`primaryRepositories`

CiProduct.Relationships.PrimaryRepositories

The related primary repository.

`bundleId`

CiProduct.Relationships.BundleId

The related bundle ID.

`additionalRepositories`

CiProduct.Relationships.AdditionalRepositories

`buildRuns`

CiProduct.Relationships.BuildRuns

`workflows`

CiProduct.Relationships.Workflows

## Topics

### Objects

object CiProduct.Relationships.App

The data and links that describe the relationship between the Products and Apps resources.

object CiProduct.Relationships.BundleId

The data and links that describe the relationship between the Products and the Bundle IDs resources.

object CiProduct.Relationships.PrimaryRepositories

The data, links, and paging information that describe the relationship between the Products resource and the Repositories resource that represents the primary repository.

### Dictionaries

object CiProduct.Relationships.AdditionalRepositories

object CiProduct.Relationships.BuildRuns

object CiProduct.Relationships.Workflows

## See Also

### Objects

object CiProduct.Attributes

The attributes that describe a Products resource.

