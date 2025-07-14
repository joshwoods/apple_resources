

- Create ML Components
- MLModelRegressorAdaptor
-  init(contentsOf:configuration:) 

Initializer

# init(contentsOf:configuration:)

Creates a model adaptor from a CoreML model URL.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    contentsOf url: URL,
    configuration: MLModelConfiguration
) throws
```

## See Also

### Creating an adaptor

init(model: MLModel) throws

Creates a MLModel regressor adaptor from a model.

