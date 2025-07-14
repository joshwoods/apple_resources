

- Natural Language
-  NLScript 

Structure

# NLScript

The writing scripts that the Natural Language framework supports.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct NLScript
```

## Topics

### Getting standard scripts

static let arabic: NLScript

The unique identifier string for the Arabic script.

static let armenian: NLScript

The unique identifier string for the Armenian script.

static let bengali: NLScript

The unique identifier string for the Bengali script.

static let canadianAboriginalSyllabics: NLScript

The unique identifier string for the Canadian Aboriginal Syllabics.

static let cherokee: NLScript

The unique identifier string for the Cherokee script.

static let cyrillic: NLScript

The unique identifier string for the Cyrillic script.

static let devanagari: NLScript

The unique identifier string for the Devanagari script.

static let ethiopic: NLScript

The unique identifier string for the Ethiopic script.

static let georgian: NLScript

The unique identifier string for the Georgian script.

static let greek: NLScript

The unique identifier string for the Greek script.

static let gujarati: NLScript

The unique identifier string for the Gujarati script.

static let gurmukhi: NLScript

The unique identifier string for the Gurmukhi script.

static let hebrew: NLScript

The unique identifier string for the Hebrew script.

static let japanese: NLScript

The unique identifier string for the Japanese script.

static let kannada: NLScript

The unique identifier string for the Kannada script.

static let khmer: NLScript

The unique identifier string for the Khmer script.

static let korean: NLScript

The unique identifier string for the Korean script.

static let lao: NLScript

The unique identifier string for the Lao script.

static let latin: NLScript

The unique identifier string for the Latin script.

static let malayalam: NLScript

The unique identifier string for the Malayalam script.

static let mongolian: NLScript

The unique identifier string for the Mongolian script.

static let myanmar: NLScript

The unique identifier string for the Myanmar script.

static let oriya: NLScript

The unique identifier string for the Oriya script.

static let simplifiedChinese: NLScript

The unique identifier string for the simplified Chinese script.

static let sinhala: NLScript

The unique identifier string for the Sinhala script.

static let tamil: NLScript

The unique identifier string for the Tamil script.

static let telugu: NLScript

The unique identifier string for the Telugu script.

static let thai: NLScript

The unique identifier string for the Thai script.

static let tibetan: NLScript

The unique identifier string for the Tibetan script.

static let traditionalChinese: NLScript

The unique identifier string for the traditional Chinese script.

static let undetermined: NLScript

The unique identifier string for a script the Natural Language framework doesn’t recognize.

### Creating custom script tags

init(String)

Creates a language script with the given string.

init(rawValue: String)

Creates a language script with the given string as its raw value.

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

struct NLContextualEmbeddingKey

Contextual embedding keys.

