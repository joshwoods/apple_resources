

- App Store Connect API
- CiWorkflowCreateRequest
-  CiWorkflowCreateRequest.Data 

Object

# CiWorkflowCreateRequest.Data

The data element of the request you use to create a new Xcode Cloud workflow.

App Store Connect API 1.5+

``` source
object CiWorkflowCreateRequest.Data
```

## Properties

`attributes`

CiWorkflowCreateRequest.Data.Attributes

 (Required) 

The attributes that describe the request that creates a Workflows resource.

`relationships`

CiWorkflowCreateRequest.Data.Relationships

 (Required) 

The types and IDs of the related data to update.

`type`

`string`

 (Required) 

The resource type.

Value: `ciWorkflows`

## Topics

### Objects

object CiWorkflowCreateRequest.Data.Attributes

The attributes you set that describe the new Xcode Cloud workflow resource.

object CiWorkflowCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

