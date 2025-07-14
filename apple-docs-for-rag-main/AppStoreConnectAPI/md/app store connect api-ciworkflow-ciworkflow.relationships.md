

- App Store Connect API
- CiWorkflow
-  CiWorkflow.Relationships 

Object

# CiWorkflow.Relationships

The relationships of the Workflows resource you included in the request and those on which you can operate.

App Store Connect API 1.5+

``` source
object CiWorkflow.Relationships
```

## Properties

`product`

CiWorkflow.Relationships.Product

The related Products resource.

`repository`

CiWorkflow.Relationships.Repository

The workflow’s related Git repository.

`xcodeVersion`

CiWorkflow.Relationships.XcodeVersion

The related Xcode Versions resource.

`macOsVersion`

CiWorkflow.Relationships.MacOsVersion

The related macOS Versions resource.

`buildRuns`

CiWorkflow.Relationships.BuildRuns

## Topics

### Objects

object CiWorkflow.Relationships.MacOsVersion

The data and links that describe the relationship between the Workflows and the macOS Versions resources.

object CiWorkflow.Relationships.Product

The data and links that describe the relationship between the Workflows and the Products resources.

object CiWorkflow.Relationships.Repository

The data and links that describe the relationship between the Workflows and the Repositories resources.

object CiWorkflow.Relationships.XcodeVersion

The data and links that describe the relationship between the Workflows and the Xcode Versions resources.

### Dictionaries

object CiWorkflow.Relationships.BuildRuns

## See Also

### Objects

object CiWorkflow.Attributes

The attributes that describe a Workflows resource.

