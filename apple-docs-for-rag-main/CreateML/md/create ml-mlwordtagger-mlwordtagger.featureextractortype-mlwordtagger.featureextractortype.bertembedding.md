

- Create ML
- MLWordTagger
- MLWordTagger.FeatureExtractorType
-  MLWordTagger.FeatureExtractorType.bertEmbedding 

Case

# MLWordTagger.FeatureExtractorType.bertEmbedding

A feature extractor that provides BERT contextual word embeddings.

macOS 14.0+

``` source
case bertEmbedding
```

## Discussion

The embeddings consider the context from left-to-right and right-to-left simultaneously.

BERT embedding requires certain downloadable assets to be present on device at training time. Training will throw an error if the specified language is unavailable at runtime. Asset downloads are managed in the background automatically by the OS when a new language is configured in device settings, such as when adding a new keyboard language or changing the preferred language.

## See Also

### Selecting a feature extractor type

case elmoEmbedding

A feature extractor that provides ELMo contextual word embeddings.

case dynamicEmbedding

A feature extractor that provides embeddings for words, based on their in-context use.

Deprecated

