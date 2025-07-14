

- App Store Connect API
- CiWorkflowCreateRequest
- 
  - CiWorkflowCreateRequest
- CiWorkflowCreateRequest.Data
- CiWorkflowCreateRequest.Data.Relationships
- CiWorkflowCreateRequest.Data.Relationships.Product
-  CiWorkflowCreateRequest.Data.Relationships.Product.Data 

Object

# CiWorkflowCreateRequest.Data.Relationships.Product.Data

The type and ID of the Products resource that you’re relating with the Workflows resource you’re creating.

App Store Connect API 1.5+

``` source
object CiWorkflowCreateRequest.Data.Relationships.Product.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Products resource.

`type`

`string`

 (Required) 

The resource type.

Value: `ciProducts`

