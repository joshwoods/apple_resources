

- Create ML
- MLImageClassifier
- MLImageClassifier.FeatureExtractorType
-  MLImageClassifier.FeatureExtractorType.custom(\_:) 

Case

# MLImageClassifier.FeatureExtractorType.custom(\_:)

A feature extractor that you provide as a Core ML model file or a layer within that file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case custom(MLImageClassifier.CustomFeatureExtractor)
```

## Parameters 

`_`  

Custom feature extractor to be used for extracting features.

## Discussion

A custom feature extractor is a neural network model you provide to an MLImageClassifier. The feature extractor can be a layer within the model or the model itself. In either case, the neural network must take an image as input and output an MLMultiArray.

## See Also

### Selecting a feature extractor type

case scenePrint(revision: Int?)

A feature extractor trained on millions of images.

struct CustomFeatureExtractor

A custom feature extractor a training session uses to train an image classifier.

