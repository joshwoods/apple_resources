

- App Store Connect API
-  ScmGitReferencesResponse 

Object

# ScmGitReferencesResponse

A response that contains a list of Git References resources.

App Store Connect API 1.5+

``` source
object ScmGitReferencesResponse
```

## Properties

`data`

`[`ScmGitReference`]`

 (Required) 

The resource data.

`included`

`[`ScmRepository`]`

The requested relationship data.

`links`

PagedDocumentLinks

 (Required) 

The navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## See Also

### Objects

object ScmGitReference

The data structure that represents a Git References resource.

object ScmGitReferenceResponse

A response that contains a single Git References resource.

