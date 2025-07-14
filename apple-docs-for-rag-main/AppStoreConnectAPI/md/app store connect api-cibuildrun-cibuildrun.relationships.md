

- App Store Connect API
- CiBuildRun
-  CiBuildRun.Relationships 

Object

# CiBuildRun.Relationships

The relationships of the Build Runs resource you included in the request and those on which you can operate.

App Store Connect API 1.5+

``` source
object CiBuildRun.Relationships
```

## Properties

`destinationBranch`

CiBuildRun.Relationships.DestinationBranch

The data and links that describe the relationship between the Build Runs resource and the Git References resource that represents the destination branch.

`product`

CiBuildRun.Relationships.Product

The data and links that describe the relationship between the Build Runs and the Products resources.

`pullRequest`

CiBuildRun.Relationships.PullRequest

The data and links that describe the relationship between the Build Runs and the Pull Requests resources.

`sourceBranchOrTag`

CiBuildRun.Relationships.SourceBranchOrTag

The data and links that describe the relationship between the Build Runs resource and the Git References resource that represents the source branch or tag.

`workflow`

CiBuildRun.Relationships.Workflow

The data and links that describe the relationship between the Build Runs and the Workflows resources.

`builds`

CiBuildRun.Relationships.Builds

The data and links that describe the relationship between the Build Runs and the Builds resources.

`actions`

CiBuildRun.Relationships.Actions

## Topics

### Objects

object CiBuildRun.Relationships.Builds

The data, links, and paging information that describe the relationship between the Build Runs and the Builds resources.

object CiBuildRun.Relationships.DestinationBranch

The data and links that describe the relationship between the Build Runs resource and the Git References resource that represents the destination branch.

object CiBuildRun.Relationships.Product

The data and links that describe the relationship between the Build Runs and the Products resources.

object CiBuildRun.Relationships.PullRequest

The data and links that describe the relationship between the Build Runs and the Pull Requests resources.

object CiBuildRun.Relationships.SourceBranchOrTag

The data and links that describe the relationship between the Build Runs and the Git References resources.

object CiBuildRun.Relationships.Workflow

The data and links that describe the relationship between the Build Runs and the Workflows resources.

### Dictionaries

object CiBuildRun.Relationships.Actions

## See Also

### Objects

object CiBuildRun.Attributes

The attributes that describe a Build Runs resource.

