

- Create ML Components
- ModelCompatibilityError
-  ModelCompatibilityError.missingPredictedFeature 

Case

# ModelCompatibilityError.missingPredictedFeature

An error that indicates that the regressor model output is missing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
case missingPredictedFeature
```

## See Also

### Analyzing the error

case incompatibleInputCount(expected: Int, actual: Int)

An error that indicates that the number of model inputs is wrong.

case incompatibleInputDataFormat(expected: MLFeatureType, actual: MLFeatureType)

An error that indicates that the input data has the wrong format.

case incompatibleInputMultiArrayDataType(MLMultiArrayDataType)

An error that indicates that the input multi array has the wrong value type.

case incompatibleLabelType

An error that indicates that the label has the wrong type.

case incompatibleMetadataKey(name: String)

An error that indicates that the metadata key has the wrong type.

case incompatibleOutputCount(expected: Int, actual: Int)

An error that indicates that the number of model outputs is wrong.

case incompatibleOutputDataFormat(expected: MLFeatureType, actual: MLFeatureType)

An error that indicates that the output data has the wrong format.

case missingInput(name: String)

An error that indicates that the input is missing from the model.

case missingLabel

An error that indicates that the label output is missing from the model.

case missingLabelProbabilities

An error that indicates that the label probabilities output is missing from the model.

case missingOutput(name: String)

An error that indicates that the output is missing from the model.

var errorDescription: String?

A localized message describing what error occurred.

