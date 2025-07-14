

- Natural Language
-  NLContextualEmbeddingKey 

Structure

# NLContextualEmbeddingKey

Contextual embedding keys.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct NLContextualEmbeddingKey
```

## Topics

### Getting embedding keys

static let languages: NLContextualEmbeddingKey

A key that identifies the languages in a contextual embedding.

static let revision: NLContextualEmbeddingKey

A key that identifies the revision for a contextual embedding.

static let scripts: NLContextualEmbeddingKey

A key that identifies the scripts in a contextual embedding.

### Creating embedding keys

init(String)

Creates an embedding key with the given string.

init(rawValue: String)

Creates an embedding key with the given string as its raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Contextual embedding

class NLContextualEmbedding

A model that computes sequences of embedding vectors for natural language utterances.

struct NLScript

The writing scripts that the Natural Language framework supports.

