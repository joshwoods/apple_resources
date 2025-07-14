

- App Store Connect API
-  ScmRepositoryResponse 

Object

# ScmRepositoryResponse

A response that contains a single Repositories resource.

App Store Connect API 1.5+

``` source
object ScmRepositoryResponse
```

## Properties

`data`

ScmRepository

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: ScmProvider`, `ScmGitReference

`links`

DocumentLinks

 (Required) 

The navigational links that include the self-link.

## See Also

### Objects

object ScmRepository

The data structure that represents a Repositories resource.

object ScmRepositoriesResponse

A response that contains a list of Repositories resources.

