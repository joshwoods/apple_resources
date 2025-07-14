

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelAlgorithmType
-  MLTextClassifier.ModelAlgorithmType.maxEnt(revision:) 

Case

# MLTextClassifier.ModelAlgorithmType.maxEnt(revision:)

A text classification algorithm that uses multinomial logistic regression based on the frequencies of words, independent of context.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
case maxEnt(revision: Int?)
```

## Parameters 

`revision`  

The algorithm version. The only supported version is 1. If `nil` defaults to the latest version.

## Mentioned in 

Creating a text classifier model

## See Also

### Selecting an algorithm type

case crf(revision: Int?)

A text classification algorithm that uses a statistical model of transition probabilities between words.

case transferLearning(MLTextClassifier.FeatureExtractorType, revision: Int?)

A text classification algorithm that uses transfer learning by leveraging a feature extractor to generate embeddings.

enum FeatureExtractorType

The text feature extractor type.

