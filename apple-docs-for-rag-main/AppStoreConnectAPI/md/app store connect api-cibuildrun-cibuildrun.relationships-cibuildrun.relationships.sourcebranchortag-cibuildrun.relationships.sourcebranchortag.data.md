

- App Store Connect API
- CiBuildRun
- CiBuildRun.Relationships
- CiBuildRun.Relationships.SourceBranchOrTag
-  CiBuildRun.Relationships.SourceBranchOrTag.Data 

Object

# CiBuildRun.Relationships.SourceBranchOrTag.Data

The type and ID of a related Git References resource that represents the source branch or tag.

App Store Connect API 1.5+

``` source
object CiBuildRun.Relationships.SourceBranchOrTag.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Git References resource that represents the source branch or tag.

`type`

`string`

 (Required) 

The resource type.

Value: `scmGitReferences`

