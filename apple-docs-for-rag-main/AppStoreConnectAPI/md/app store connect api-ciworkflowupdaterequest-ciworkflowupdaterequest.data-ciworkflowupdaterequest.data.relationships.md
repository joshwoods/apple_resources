

- App Store Connect API
- CiWorkflowUpdateRequest
- CiWorkflowUpdateRequest.Data
-  CiWorkflowUpdateRequest.Data.Relationships 

Object

# CiWorkflowUpdateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

App Store Connect API 1.5+

``` source
object CiWorkflowUpdateRequest.Data.Relationships
```

## Properties

`xcodeVersion`

CiWorkflowUpdateRequest.Data.Relationships.XcodeVersion

The related Xcode Versions resource.

`macOsVersion`

CiWorkflowUpdateRequest.Data.Relationships.MacOsVersion

The related macOS Versions resource.

## Topics

### Objects

object CiWorkflowUpdateRequest.Data.Relationships.MacOsVersion

The relationship to the macOS Versions resource you can set with the request that updates a Workflows resource.

object CiWorkflowUpdateRequest.Data.Relationships.XcodeVersion

The relationship to the Xcode Versions resource you can set with the request that updates a Workflows resource.

## See Also

### Objects

object CiWorkflowUpdateRequest.Data.Attributes

The attributes of the Workflows resource you’re changing with the update request.

