

- Natural Language
- NLModel
-  init(mlModel:) 

Initializer

# init(mlModel:)

Creates a new natural language model based on the given Core ML model instance.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
convenience init(mlModel: MLModel) throws
```

## Parameters 

`mlModel`  

A Core ML model instance that’s the basis for this natural language model.

## See Also

### Creating a model

convenience init(contentsOf: URL) throws

Creates a new natural language model based on a compiled Core ML model at the given URL.

