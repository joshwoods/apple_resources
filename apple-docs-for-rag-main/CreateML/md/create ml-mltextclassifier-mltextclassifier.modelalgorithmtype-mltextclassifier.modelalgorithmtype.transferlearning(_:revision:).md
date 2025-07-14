

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelAlgorithmType
-  MLTextClassifier.ModelAlgorithmType.transferLearning(\_:revision:) 

Case

# MLTextClassifier.ModelAlgorithmType.transferLearning(\_:revision:)

A text classification algorithm that uses transfer learning by leveraging a feature extractor to generate embeddings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case transferLearning(
    MLTextClassifier.FeatureExtractorType,
    revision: Int?
)
```

## Parameters 

`_`  

Feature extractor to be used by the transfer learning algorithm.

`revision`  

The algorithm version. The only supported version is 1. If `nil` defaults to the latest version.

## Mentioned in 

Creating a text classifier model

## See Also

### Selecting an algorithm type

case crf(revision: Int?)

A text classification algorithm that uses a statistical model of transition probabilities between words.

case maxEnt(revision: Int?)

A text classification algorithm that uses multinomial logistic regression based on the frequencies of words, independent of context.

enum FeatureExtractorType

The text feature extractor type.

