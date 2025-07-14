

- App Store Connect API
-  ScmPullRequestResponse 

Object

# ScmPullRequestResponse

A response that contains a single Pull Requests resource.

App Store Connect API 1.5+

``` source
object ScmPullRequestResponse
```

## Properties

`data`

ScmPullRequest

 (Required) 

The resource data.

`included`

`[`ScmRepository`]`

The requested relationship data.

`links`

DocumentLinks

 (Required) 

The navigational links that include the self-link.

## See Also

### Objects

object ScmPullRequest

The data structure that represents a Pull Requests resource.

object ScmPullRequestsResponse

A response that contains a list of Pull Requests resources.

