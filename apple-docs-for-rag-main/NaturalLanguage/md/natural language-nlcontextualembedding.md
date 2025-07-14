

- Natural Language
-  NLContextualEmbedding 

Class

# NLContextualEmbedding

A model that computes sequences of embedding vectors for natural language utterances.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class NLContextualEmbedding
```

## Overview

Starting in iOS 17 and macOS 14, the framework supports 27 languages across three models:

- Latin — including Croatian, Czech, Danish, Dutch, English, Finnish, French, German, Hungarian, Indonesian, Italian, Norwegian, Polish, Portuguese, Romanian, Slovak, Swedish, Spanish, Turkish, and Vietnamese

- Cyrillic — including Bulgarian, Kazakh, Russian, and Ukrainian

- Chinese, Japanese, and Korean

In iOS 18 and macOS 15, the framework expands language support to include three additional models:

- Arabic

- Thai

- Indic — including Hindi, Marathi, Bangla, Urdu, Punjabi, Gujarati, Tamil, Telugu, Kannada, and Malayalam

## Topics

### Creating a contextual embedding

convenience init?(modelIdentifier: String)

Creates a contextual embedding from a model identifier.

init?(language: NLLanguage)

Creates a contextual embedding from a language.

init?(script: NLScript)

Creates a contextual embedding from a script.

### Inspecting the contextual embedding

var dimension: Int

The number of dimensions in the script’s vector space.

var hasAvailableAssets: Bool

A Boolean value that indicates whether assets are available to load.

var languages: [NLLanguage]

The languages of the text in the contextual embedding.

var maximumSequenceLength: Int

The maximum number of embedding vectors the model generates, in sequence.

var modelIdentifier: String

The model identifier.

var revision: Int

The revision of the contextual embedding.

var scripts: [NLScript]

The scripts of the text in the contextual embedding.

### Requesting assets

func requestAssets(completionHandler: (NLContextualEmbedding.AssetsResult, (any Error)?) -> Void)

Requests assets for an embedding, if available.

enum AssetsResult

The status of an asset request.

### Loading and unloading assets

func load() throws

Loads the embedding model.

func unload()

Unloads the embedding model.

### Applying an embedding

func embeddingResult(for: String, language: NLLanguage?) throws -> NLContextualEmbeddingResult

Applies an embedding to a string and obtains the resulting embedding vectors.

class NLContextualEmbeddingResult

An object that represents the embedding vector result from applying a contextual embedding to a string.

### Type Methods

class func contextualEmbeddings(forValues: [NLContextualEmbeddingKey : Any]) -> [NLContextualEmbedding]

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

### Contextual embedding

struct NLContextualEmbeddingKey

Contextual embedding keys.

struct NLScript

The writing scripts that the Natural Language framework supports.

