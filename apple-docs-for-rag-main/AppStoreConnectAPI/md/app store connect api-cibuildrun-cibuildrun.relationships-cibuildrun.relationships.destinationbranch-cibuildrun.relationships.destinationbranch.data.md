

- App Store Connect API
- CiBuildRun
- CiBuildRun.Relationships
- CiBuildRun.Relationships.DestinationBranch
-  CiBuildRun.Relationships.DestinationBranch.Data 

Object

# CiBuildRun.Relationships.DestinationBranch.Data

The type and ID of a related Git References resource that represents the build run’s destination branch.

App Store Connect API 1.5+

``` source
object CiBuildRun.Relationships.DestinationBranch.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Git References resource that represents the destination branch.

`type`

`string`

 (Required) 

The resource type.

Value: `scmGitReferences`

