

- Vision
- VNCoreMLModel
-  init(for:) 

Initializer

# init(for:)

Creates a model container to use with a Core ML request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
convenience init(for model: MLModel) throws
```

## Parameters 

`model`  

The model to create the model container from.

## Discussion

This method may fail if the framework doesn’t support the Core ML model. For example, a model that doesn’t accept an image as any of its inputs will yield an VNErrorCode.invalidModel error.

