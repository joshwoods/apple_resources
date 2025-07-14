

- App Store Connect API
- CiWorkflowCreateRequest
- 
  - CiWorkflowCreateRequest
- CiWorkflowCreateRequest.Data
- CiWorkflowCreateRequest.Data.Relationships
- CiWorkflowCreateRequest.Data.Relationships.Repository
-  CiWorkflowCreateRequest.Data.Relationships.Repository.Data 

Object

# CiWorkflowCreateRequest.Data.Relationships.Repository.Data

The type and ID of the Repositories resource that you’re relating with the Workflows resource you’re creating.

App Store Connect API 1.5+

``` source
object CiWorkflowCreateRequest.Data.Relationships.Repository.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Repositories resource.

`type`

`string`

 (Required) 

The resource type.

Value: `scmRepositories`

