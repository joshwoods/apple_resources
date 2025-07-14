

- App Store Connect API
- CiBuildRunCreateRequest
- CiBuildRunCreateRequest.Data
- CiBuildRunCreateRequest.Data.Relationships
-  CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag 

Object

# CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag

The relationship to the Git References resource that represents the source branch or tag you can set with the request that creates a Build Runs resource.

App Store Connect API 1.5+

``` source
object CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag
```

## Properties

`data`

CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag.Data

The ID and type of the related Git References resource that represents the source branch or tag.

## Topics

### Objects

object CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag.Data

The type and ID of the Git References resource that represents the source branch or tag you relate with the Build Runs resource you’re creating.

## See Also

### Objects

object CiBuildRunCreateRequest.Data.Relationships.BuildRun

The relationship to the Build Runs resource you can set with the request that creates a Build Runs resource.

object CiBuildRunCreateRequest.Data.Relationships.PullRequest

The relationship to the Pull Requests resource you can set with the request that creates a Build Runs resource.

object CiBuildRunCreateRequest.Data.Relationships.Workflow

The relationship to the Workflows resource you can set with the request that creates a Build Runs resource.

