

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
- MLObjectDetector.ModelParameters.ModelAlgorithmType
-  MLObjectDetector.ModelParameters.ModelAlgorithmType.transferLearning(\_:) 

Case

# MLObjectDetector.ModelParameters.ModelAlgorithmType.transferLearning(\_:)

An algorithm that leverages the knowledge of a general purpose model built into the operating system.

macOS 11.0+

``` source
case transferLearning(MLObjectDetector.ModelParameters.FeatureExtractorType)
```

## Discussion

You typically use this transfer-learning algorithm to train an object detector in these situations:

- Your training dataset has a limited number of examples. - You prefer your object detector’s Core ML model file to be as small as possible.

## See Also

### Designating an algorithm

case darknetYolo

An algorithm that trains a full neural network with your training data.

enum FeatureExtractorType

The underlying base model that extracts image features for an object-detector training session.

