

- App Store Connect API
- CiWorkflowCreateRequest
- CiWorkflowCreateRequest.Data
-  CiWorkflowCreateRequest.Data.Relationships 

Object

# CiWorkflowCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

App Store Connect API 1.5+

``` source
object CiWorkflowCreateRequest.Data.Relationships
```

## Properties

`product`

CiWorkflowCreateRequest.Data.Relationships.Product

 (Required) 

The related Products resource.

`repository`

CiWorkflowCreateRequest.Data.Relationships.Repository

 (Required) 

The related Repositories resource.

`xcodeVersion`

CiWorkflowCreateRequest.Data.Relationships.XcodeVersion

 (Required) 

The related Xcode Versions resource.

`macOsVersion`

CiWorkflowCreateRequest.Data.Relationships.MacOsVersion

 (Required) 

The related macOS Versions resource.

## Topics

### Objects

object CiWorkflowCreateRequest.Data.Relationships.MacOsVersion

The relationship to the macOS Versions resource you set with the request that creates a Workflows resource.

object CiWorkflowCreateRequest.Data.Relationships.Product

The relationship to the Products resource you set with the request that creates a Workflows resource.

object CiWorkflowCreateRequest.Data.Relationships.Repository

The relationship to the Repositories Versions resource you set with the request that creates a Workflows resource.

object CiWorkflowCreateRequest.Data.Relationships.XcodeVersion

The relationship to the Xcode Versions resource you set with the request that creates a Workflows resource.

## See Also

### Objects

object CiWorkflowCreateRequest.Data.Attributes

The attributes you set that describe the new Xcode Cloud workflow resource.

