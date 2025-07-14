

- Create ML
- MLTextClassifier
- MLTextClassifier.FeatureExtractorType
-  MLTextClassifier.FeatureExtractorType.dynamicEmbedding 

Case

# MLTextClassifier.FeatureExtractorType.dynamicEmbedding

A feature extractor that provides embeddings for words, based on their in-context use.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 10.15–14.0DeprecatedvisionOS 1.0+

``` source
case dynamicEmbedding
```

## Discussion

Dynamic embedding requires certain downloadable assets to be present on device at training time. Training will throw an error if the specified language is unavailable at runtime. Asset downloads are managed in the background automatically by the OS when a new language is configured in device settings, such as when adding a new keyboard language or changing the preferred language.

## See Also

### Selecting a feature extractor type

case customEmbedding(URL)

A feature extractor that uses a custom embedding contained in a CoreML model file.

case staticEmbedding

A feature extractor that uses the standard, built-in word embeddings.

case bertEmbedding

A feature extractor that provides BERT contextual word embeddings.

case elmoEmbedding

A feature extractor that provides ELMo contextual word embeddings.

