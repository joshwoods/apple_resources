

- App Store Connect API
- CiWorkflowCreateRequest
- 
  - CiWorkflowCreateRequest
- CiWorkflowCreateRequest.Data
- CiWorkflowCreateRequest.Data.Relationships
- CiWorkflowCreateRequest.Data.Relationships.MacOsVersion
-  CiWorkflowCreateRequest.Data.Relationships.MacOsVersion.Data 

Object

# CiWorkflowCreateRequest.Data.Relationships.MacOsVersion.Data

The type and ID of the macOS Versions resource that you’re relating with the Workflows resource you’re creating.

App Store Connect API 1.5+

``` source
object CiWorkflowCreateRequest.Data.Relationships.MacOsVersion.Data
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

