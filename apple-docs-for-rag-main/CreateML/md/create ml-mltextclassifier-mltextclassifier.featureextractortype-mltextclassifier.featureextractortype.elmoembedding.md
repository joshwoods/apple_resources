

- Create ML
- MLTextClassifier
- MLTextClassifier.FeatureExtractorType
-  MLTextClassifier.FeatureExtractorType.elmoEmbedding 

Case

# MLTextClassifier.FeatureExtractorType.elmoEmbedding

A feature extractor that provides ELMo contextual word embeddings.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
case elmoEmbedding
```

## Mentioned in 

Creating a text classifier model

## Discussion

ELMo embeddings requires certain downloadable assets to be present on device at training time. Training will throw an error if the specified language is unavailable at runtime. Asset downloads are managed in the background automatically by the OS when a new language is configured in device settings, such as when adding a new keyboard language or changing the preferred language.

## See Also

### Selecting a feature extractor type

case customEmbedding(URL)

A feature extractor that uses a custom embedding contained in a CoreML model file.

case staticEmbedding

A feature extractor that uses the standard, built-in word embeddings.

case bertEmbedding

A feature extractor that provides BERT contextual word embeddings.

case dynamicEmbedding

A feature extractor that provides embeddings for words, based on their in-context use.

