

- Natural Language
- NLContextualEmbeddingResult
-  tokenVector(at:) 

Instance Method

# tokenVector(at:)

Gets a token vector at the index you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@nonobjc
func tokenVector(at index: String.Index) -> ([Double], Range)?
```

## Parameters 

`index`  

The index to get the token vector at.

## See Also

### Enumerating the vectors

func enumerateTokenVectors(in: Range&lt;String.Index>, using: ([Double], Range&lt;String.Index>) -> Bool)

Iterates over the embedding vectors for the range you specify.

