

- App Store Connect API
- CiBuildRun
- CiBuildRun.Relationships
-  CiBuildRun.Relationships.Builds 

Object

# CiBuildRun.Relationships.Builds

The data, links, and paging information that describe the relationship between the Build Runs and the Builds resources.

App Store Connect API 1.5+

``` source
object CiBuildRun.Relationships.Builds
```

## Properties

`data`

`[`CiBuildRun.Relationships.Builds.Data`]`

The ID and type of the related Builds resource.

`links`

RelationshipLinks

The navigational links that include the self-link.

`meta`

PagingInformation

The paging information.

## Topics

### Objects

object CiBuildRun.Relationships.Builds.Data

The type and ID of a related Builds resource.

## See Also

### Objects

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

