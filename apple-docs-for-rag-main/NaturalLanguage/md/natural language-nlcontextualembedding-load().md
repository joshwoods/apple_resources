

- Natural Language
- NLContextualEmbedding
-  load() 

Instance Method

# load()

Loads the embedding model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func load() throws
```

## Discussion

When you create a contextual embedding, the model isn’t loaded until you need it, by default. Use load() and unload() to control when to load and unload the model.

The method fails if the necessary assets — for the model you specify — aren’t on device. Use hasAvailableAssets and requestAssets(completionHandler:) to manage the assets.

## See Also

### Loading and unloading assets

func unload()

Unloads the embedding model.

