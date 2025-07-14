

- Create ML Components
- MLModelImageFeatureExtractor
-  init(model:inputName:outputName:context:) 

Initializer

# init(model:inputName:outputName:context:)

Creates an image feature extractor from a CoreML model.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    model: MLModel,
    inputName: String = "image",
    outputName: String,
    context: CIContext = CIContext()
) throws
```

## Parameters 

`model`  

The CoreML model which will be used for feature extraction.

`inputName`  

The name of the input which the `model` expects.

`outputName`  

The name of the output from the `model`.

`context`  

A Core Image context.

## See Also

### Creating the extractor

init(contentsOf: URL, configuration: MLModelConfiguration, inputName: String, outputName: String, context: CIContext) async throws

Creates an image feature extractor from a CoreML model URL.

