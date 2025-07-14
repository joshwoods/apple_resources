

- App Store Connect API
- CiWorkflowCreateRequest
- 
  - CiWorkflowCreateRequest
- CiWorkflowCreateRequest.Data
- CiWorkflowCreateRequest.Data.Relationships
- CiWorkflowCreateRequest.Data.Relationships.XcodeVersion
-  CiWorkflowCreateRequest.Data.Relationships.XcodeVersion.Data 

Object

# CiWorkflowCreateRequest.Data.Relationships.XcodeVersion.Data

The type and ID of the Xcode Versions resource that you’re relating with the Workflows resource you’re creating.

App Store Connect API 1.5+

``` source
object CiWorkflowCreateRequest.Data.Relationships.XcodeVersion.Data
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

