

- Create ML
- MLTextClassifier
- MLTextClassifier.FeatureExtractorType
-  MLTextClassifier.FeatureExtractorType.customEmbedding(\_:) 

Case

# MLTextClassifier.FeatureExtractorType.customEmbedding(\_:)

A feature extractor that uses a custom embedding contained in a CoreML model file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case customEmbedding(URL)
```

## Discussion

- URL: The path to a model file (ending in `.mlmodel`, `.mlmodelc`, or `.dat`).

## See Also

### Selecting a feature extractor type

case staticEmbedding

A feature extractor that uses the standard, built-in word embeddings.

case bertEmbedding

A feature extractor that provides BERT contextual word embeddings.

case elmoEmbedding

A feature extractor that provides ELMo contextual word embeddings.

case dynamicEmbedding

A feature extractor that provides embeddings for words, based on their in-context use.

