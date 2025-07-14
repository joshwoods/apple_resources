

- App Store Connect API
-  ScmRepository 

Object

# ScmRepository

The data structure that represents a Repositories resource.

App Store Connect API 1.5+

``` source
object ScmRepository
```

## Properties

`attributes`

ScmRepository.Attributes

The attributes that describe the Repositories resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Repositories resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

ScmRepository.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `scmRepositories`

## Topics

### Objects

object ScmRepository.Attributes

The attributes that describe a Repositories resource.

object ScmRepository.Relationships

The relationships of the Repositories resource you included in the request and those on which you can operate.

## See Also

### Objects

object ScmRepositoryResponse

A response that contains a single Repositories resource.

object ScmRepositoriesResponse

A response that contains a list of Repositories resources.

