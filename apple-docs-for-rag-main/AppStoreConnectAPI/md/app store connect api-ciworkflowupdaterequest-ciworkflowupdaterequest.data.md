

- App Store Connect API
- CiWorkflowUpdateRequest
-  CiWorkflowUpdateRequest.Data 

Object

# CiWorkflowUpdateRequest.Data

The data element of the request you use to update an Xcode Cloud workflow.

App Store Connect API 1.5+

``` source
object CiWorkflowUpdateRequest.Data
```

## Properties

`attributes`

CiWorkflowUpdateRequest.Data.Attributes

The attributes that describe the request that updates a Workflows resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the request.

`relationships`

CiWorkflowUpdateRequest.Data.Relationships

The types and IDs of the related data to update.

`type`

`string`

 (Required) 

The resource type.

Value: `ciWorkflows`

## Topics

### Objects

object CiWorkflowUpdateRequest.Data.Attributes

The attributes of the Workflows resource you’re changing with the update request.

object CiWorkflowUpdateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

