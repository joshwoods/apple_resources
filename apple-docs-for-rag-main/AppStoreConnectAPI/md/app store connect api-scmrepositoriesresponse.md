

- App Store Connect API
-  ScmRepositoriesResponse 

Object

# ScmRepositoriesResponse

A response that contains a list of Repositories resources.

App Store Connect API 1.5+

``` source
object ScmRepositoriesResponse
```

## Properties

`data`

`[`ScmRepository`]`

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: ScmProvider`, `ScmGitReference

`links`

PagedDocumentLinks

 (Required) 

The navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## See Also

### Objects

object ScmRepository

The data structure that represents a Repositories resource.

object ScmRepositoryResponse

A response that contains a single Repositories resource.

