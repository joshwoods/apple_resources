

- App Store Connect API
- CiBuildRunCreateRequest
- 
  - CiBuildRunCreateRequest
- CiBuildRunCreateRequest.Data
- CiBuildRunCreateRequest.Data.Relationships
- CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag
-  CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag.Data 

Object

# CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag.Data

The type and ID of the Git References resource that represents the source branch or tag you relate with the Build Runs resource you’re creating.

App Store Connect API 1.5+

``` source
object CiBuildRunCreateRequest.Data.Relationships.SourceBranchOrTag.Data
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

