

- App Store Connect API
- ScmRepository
- ScmRepository.Relationships
- ScmRepository.Relationships.DefaultBranch
-  ScmRepository.Relationships.DefaultBranch.Data 

Object

# ScmRepository.Relationships.DefaultBranch.Data

The type and ID of a related Git References resource that represents the repository’s default branch.

App Store Connect API 1.5+

``` source
object ScmRepository.Relationships.DefaultBranch.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Git References resource that represents the default branch.

`type`

`string`

 (Required) 

The resource type.

Value: `scmGitReferences`

