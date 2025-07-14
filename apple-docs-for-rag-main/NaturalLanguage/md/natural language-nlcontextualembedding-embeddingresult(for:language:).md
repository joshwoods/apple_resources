

- Natural Language
- NLContextualEmbedding
-  embeddingResult(for:language:) 

Instance Method

# embeddingResult(for:language:)

Applies an embedding to a string and obtains the resulting embedding vectors.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func embeddingResult(
    for string: String,
    language: NLLanguage?
) throws -> NLContextualEmbeddingResult
```

## Parameters 

`string`  

The string to apply an embedding to.

`language`  

The language of the string.

## Return Value

An embedding result.

## Discussion

If the language of the string is unknown, the framework infers it from the string you specify.

## See Also

### Applying an embedding

class NLContextualEmbeddingResult

An object that represents the embedding vector result from applying a contextual embedding to a string.

