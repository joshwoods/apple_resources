

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
- MLObjectDetector.ModelParameters.ModelAlgorithmType
-  MLObjectDetector.ModelParameters.ModelAlgorithmType.darknetYolo 

Case

# MLObjectDetector.ModelParameters.ModelAlgorithmType.darknetYolo

An algorithm that trains a full neural network with your training data.

macOS 11.0+

``` source
case darknetYolo
```

## Discussion

Use this algorithm when your training dataset has a significant number of examples.

## See Also

### Designating an algorithm

case transferLearning(MLObjectDetector.ModelParameters.FeatureExtractorType)

An algorithm that leverages the knowledge of a general purpose model built into the operating system.

enum FeatureExtractorType

The underlying base model that extracts image features for an object-detector training session.

