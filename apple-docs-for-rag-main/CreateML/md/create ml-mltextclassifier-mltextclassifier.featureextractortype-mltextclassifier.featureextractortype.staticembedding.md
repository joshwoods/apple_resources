

- Create ML
- MLTextClassifier
- MLTextClassifier.FeatureExtractorType
-  MLTextClassifier.FeatureExtractorType.staticEmbedding 

Case

# MLTextClassifier.FeatureExtractorType.staticEmbedding

A feature extractor that uses the standard, built-in word embeddings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case staticEmbedding
```

## Discussion

The standard word embeddings are the same as those that NLEmbedding provides with its wordEmbedding(for:) method.

## See Also

### Selecting a feature extractor type

case customEmbedding(URL)

A feature extractor that uses a custom embedding contained in a CoreML model file.

case bertEmbedding

A feature extractor that provides BERT contextual word embeddings.

case elmoEmbedding

A feature extractor that provides ELMo contextual word embeddings.

case dynamicEmbedding

A feature extractor that provides embeddings for words, based on their in-context use.

