

- Create ML Components
- MLModelImageFeatureExtractor
-  model 

Instance Property

# model

The CoreML model with .mlmodel extension.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
let model: MLModel
```

## Discussion

This model should satisfy the following requirements:

1.  Take in one input of type .image and its key name should be same as `inputName`.

2.  Any other input should be optional.

3.  Give at least one output of type .multiarray and its key name should be same as `outputName`

## See Also

### Getting the properties

let inputName: String

The model’s input feature name.

let outputName: String

The model’s output feature name.

