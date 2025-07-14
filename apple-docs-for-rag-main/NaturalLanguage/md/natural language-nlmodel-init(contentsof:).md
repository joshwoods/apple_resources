

- Natural Language
- NLModel
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Creates a new natural language model based on a compiled Core ML model at the given URL.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
convenience init(contentsOf url: URL) throws
```

## Parameters 

`url`  

The location of the *compiled* Core ML model file in the file system (ending with `.mlmodelc`) that’s the basis for this natural language model.

## See Also

### Creating a model

convenience init(mlModel: MLModel) throws

Creates a new natural language model based on the given Core ML model instance.

