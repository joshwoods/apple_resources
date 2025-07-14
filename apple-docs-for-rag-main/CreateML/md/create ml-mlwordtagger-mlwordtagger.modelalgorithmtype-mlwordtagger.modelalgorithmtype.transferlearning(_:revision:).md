

- Create ML
- MLWordTagger
- MLWordTagger.ModelAlgorithmType
-  MLWordTagger.ModelAlgorithmType.transferLearning(\_:revision:) 

Case

# MLWordTagger.ModelAlgorithmType.transferLearning(\_:revision:)

A transfer-learning algorithm.

macOS 11.0+

``` source
case transferLearning(
    MLWordTagger.FeatureExtractorType,
    revision: Int = 1
)
```

## See Also

### Selecting an algorithm type

case crf(revision: Int?)

A conditional random field algorithm.

enum FeatureExtractorType

The feature extractors that are available to train a word tagger using with the transfer-learning algorithm option.

