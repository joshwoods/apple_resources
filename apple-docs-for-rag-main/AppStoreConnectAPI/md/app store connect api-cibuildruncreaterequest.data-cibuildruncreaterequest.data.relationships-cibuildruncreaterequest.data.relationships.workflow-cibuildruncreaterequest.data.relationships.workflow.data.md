

- App Store Connect API
- CiBuildRunCreateRequest
- 
  - CiBuildRunCreateRequest
- CiBuildRunCreateRequest.Data
- CiBuildRunCreateRequest.Data.Relationships
- CiBuildRunCreateRequest.Data.Relationships.Workflow
-  CiBuildRunCreateRequest.Data.Relationships.Workflow.Data 

Object

# CiBuildRunCreateRequest.Data.Relationships.Workflow.Data

The type and ID of the Workflows resource that you’re relating with the Build Runs resource you’re creating.

App Store Connect API 1.5+

``` source
object CiBuildRunCreateRequest.Data.Relationships.Workflow.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Workflows resource.

`type`

`string`

 (Required) 

The resource type.

Value: `ciWorkflows`

