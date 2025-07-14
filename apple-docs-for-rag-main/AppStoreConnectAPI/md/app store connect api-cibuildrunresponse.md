

- App Store Connect API
-  CiBuildRunResponse 

Object

# CiBuildRunResponse

A response that contains a single Build Runs resource.

App Store Connect API 1.5+

``` source
object CiBuildRunResponse
```

## Properties

`data`

CiBuildRun

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: Build`, `CiWorkflow`, `CiProduct`, `ScmGitReference`, `ScmPullRequest

`links`

DocumentLinks

 (Required) 

The navigational links that include the self-link.

## See Also

### Objects

object CiBuildRun

The data structure that represents a Build Runs resource.

object CiBuildRunCreateRequest

The request body you use to start a new Xcode Cloud build.

object CiBuildActionsResponse

A response that contains a list of Build Actions resources.

