

- Core ML
- MLCustomModel
-  init(modelDescription:parameters:) 

Initializer

# init(modelDescription:parameters:)

Creates a custom model with the given description and parameters.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init(
    modelDescription: MLModelDescription,
    parameters: [String : Any]
) throws
```

**Required**

## Parameters 

`modelDescription`  

A description of the model.

`parameters`  

The parameters for configuring the model.

