

- App Store Connect API
- CiBuildRunCreateRequest
- CiBuildRunCreateRequest.Data
-  CiBuildRunCreateRequest.Data.Relationships 

Object

# CiBuildRunCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

App Store Connect API 1.5+

``` source
object CiBuildRunCreateRequest.Data.Relationships
```

## Properties

`workflow`

CiBuildRunCreateRequest.Data.Relationships.Workflow

The related Workflows resource.

`buildRun`

CiBuildRunCreateRequest.Data.Relationships.BuildRun

The related Build Runs resource.

`pullRequest`

CiBuildRunCreateRequest.Data.Relationships.PullRequest

The related Pull Requests resource.

`sourceBranchOrTag`

CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag

The related Git References resource.

## Topics

### Objects

object CiBuildRunCreateRequest.Data.Relationships.BuildRun

The relationship to the Build Runs resource you can set with the request that creates a Build Runs resource.

object CiBuildRunCreateRequest.Data.Relationships.PullRequest

The relationship to the Pull Requests resource you can set with the request that creates a Build Runs resource.

object CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag

The relationship to the Git References resource that represents the source branch or tag you can set with the request that creates a Build Runs resource.

object CiBuildRunCreateRequest.Data.Relationships.Workflow

The relationship to the Workflows resource you can set with the request that creates a Build Runs resource.

## See Also

### Objects

object CiBuildRunCreateRequest.Data.Attributes

The attributes you set that describe the new Build Runs resource.

