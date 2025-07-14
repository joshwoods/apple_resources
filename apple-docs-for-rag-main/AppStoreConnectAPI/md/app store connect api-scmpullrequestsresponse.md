

- App Store Connect API
-  ScmPullRequestsResponse 

Object

# ScmPullRequestsResponse

A response that contains a list of Pull Requests resources.

App Store Connect API 1.5+

``` source
object ScmPullRequestsResponse
```

## Properties

`data`

`[`ScmPullRequest`]`

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

object ScmPullRequest

The data structure that represents a Pull Requests resource.

object ScmPullRequestResponse

A response that contains a single Pull Requests resource.

