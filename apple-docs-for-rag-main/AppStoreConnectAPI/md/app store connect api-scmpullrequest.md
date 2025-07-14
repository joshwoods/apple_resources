

- App Store Connect API
-  ScmPullRequest 

Object

# ScmPullRequest

The data structure that represents a Pull Requests resource.

App Store Connect API 1.5+

``` source
object ScmPullRequest
```

## Properties

`attributes`

ScmPullRequest.Attributes

The attributes that describe the Pull Requests resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Pull Request resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

ScmPullRequest.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `scmPullRequests`

## Topics

### Objects

object ScmPullRequest.Attributes

The attributes that describe a Pull Requests resource.

object ScmPullRequest.Relationships

The relationships of the Pull Requests resource you included in the request and those on which you can operate.

## See Also

### Objects

object ScmPullRequestResponse

A response that contains a single Pull Requests resource.

object ScmPullRequestsResponse

A response that contains a list of Pull Requests resources.

