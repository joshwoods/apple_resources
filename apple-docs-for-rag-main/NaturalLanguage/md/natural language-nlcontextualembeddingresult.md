

- Natural Language
-  NLContextualEmbeddingResult 

Class

# NLContextualEmbeddingResult

An object that represents the embedding vector result from applying a contextual embedding to a string.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class NLContextualEmbeddingResult
```

## Topics

### Inspecting the result

var language: NLLanguage

The resulting language.

var sequenceLength: Int

The number of embedding vectors the request generates.

var string: String

The string value.

### Enumerating the vectors

func enumerateTokenVectors(in: Range&lt;String.Index>, using: ([Double], Range&lt;String.Index>) -> Bool)

Iterates over the embedding vectors for the range you specify.

func tokenVector(at: String.Index) -> ([Double], Range&lt;String.Index>)?

Gets a token vector at the index you specify.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Applying an embedding

func embeddingResult(for: String, language: NLLanguage?) throws -> NLContextualEmbeddingResult

Applies an embedding to a string and obtains the resulting embedding vectors.

