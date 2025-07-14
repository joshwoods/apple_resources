

- App Store Connect API
- CiWorkflowUpdateRequest
- 
  - CiWorkflowUpdateRequest
- CiWorkflowUpdateRequest.Data
- CiWorkflowUpdateRequest.Data.Relationships
- CiWorkflowUpdateRequest.Data.Relationships.XcodeVersion
-  CiWorkflowUpdateRequest.Data.Relationships.XcodeVersion.Data 

Object

# CiWorkflowUpdateRequest.Data.Relationships.XcodeVersion.Data

The type and ID of the Xcode Versions resource that you’re relating with the Workflows resource you’re updating.

App Store Connect API 1.5+

``` source
object CiWorkflowUpdateRequest.Data.Relationships.XcodeVersion.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related Xcode Versions resource.

`type`

`string`

 (Required) 

The resource type.

Value: `ciXcodeVersions`

