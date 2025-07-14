

- Natural Language
- NLContextualEmbeddingResult
-  enumerateTokenVectors(in:using:) 

Instance Method

# enumerateTokenVectors(in:using:)

Iterates over the embedding vectors for the range you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@nonobjc
func enumerateTokenVectors(
    in range: Range,
    using block: ([Double], Range) -> Bool
)
```

## Parameters 

`range`  

The range in the string to enumerate.

`block`  

A block that contains the token vectors and the token’s range.

## See Also

### Enumerating the vectors

func tokenVector(at: String.Index) -> ([Double], Range&lt;String.Index>)?

Gets a token vector at the index you specify.

