

- Create ML
- MLWordTagger
- MLWordTagger.FeatureExtractorType
-  MLWordTagger.FeatureExtractorType.dynamicEmbedding Deprecated

Case

# MLWordTagger.FeatureExtractorType.dynamicEmbedding

A feature extractor that provides embeddings for words, based on their in-context use.

macOS 11.0–14.0Deprecated

``` source
case dynamicEmbedding
```

## Discussion

Dynamic embedding requires certain downloadable assets to be present on device at training time. Training will throw an error if the specified language is unavailable at runtime. Asset downloads are managed in the background automatically by the OS when a new language is configured in device settings, such as when adding a new keyboard language or changing the preferred language.

## See Also

### Selecting a feature extractor type

case bertEmbedding

A feature extractor that provides BERT contextual word embeddings.

case elmoEmbedding

A feature extractor that provides ELMo contextual word embeddings.

