

- App Store Connect API
- CiWorkflowUpdateRequest
- 
  - CiWorkflowUpdateRequest
- CiWorkflowUpdateRequest.Data
- CiWorkflowUpdateRequest.Data.Relationships
- CiWorkflowUpdateRequest.Data.Relationships.MacOsVersion
-  CiWorkflowUpdateRequest.Data.Relationships.MacOsVersion.Data 

Object

# CiWorkflowUpdateRequest.Data.Relationships.MacOsVersion.Data

The type and ID of the macOS Versions resource that you’re relating with the Workflows resource you’re updating.

App Store Connect API 1.5+

``` source
object CiWorkflowUpdateRequest.Data.Relationships.MacOsVersion.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the related macOS Versions resource.

`type`

`string`

 (Required) 

The resource type.

Value: `ciMacOsVersions`

