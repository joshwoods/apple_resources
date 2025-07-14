

- Natural Language
-  NLTagScheme 

Structure

# NLTagScheme

Constants for the tag schemes specified when initializing a linguistic tagger.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct NLTagScheme
```

## Mentioned in 

Creating a word tagger model

## Overview

When initializing a linguistic tagger with init(_:), you specify one or more tag schemes that correspond to the kind of information you’re interested in for a selection of natural language text. To ensure optimal performance, avoid specifying tag schemes that you won’t use.

Some tag schemes are only available for certain units and languages. Use availableTagSchemes(for:language:) to determine the possible values for a specified language and linguistic unit.

When working with linguistic tags using the methods described in Getting linguistic tags and Enumerating linguistic tags in NLTagger, the returned tag value depends on the specified scheme. For example, given the token “Überraschung”, the returned tag is noun when using the lexicalClass tag scheme, german (German language) when using the language tag scheme, and “Latn” (Latin script) when using the script tag scheme, as shown in the following code.

```
let tagger = NLTagger(tagSchemes: [.lexicalClass, .language, .script], options: 0)
tagger.string = "Überraschung"

tagger.tag(at: 0, unit: .word, scheme: .lexicalClass, tokenRange: nil) // Noun
tagger.tag(at: 0, unit: .word, scheme: .language, tokenRange: nil) // german
tagger.tag(at: 0, unit: .word, scheme: .script, tokenRange: nil) // Latn
```

## Topics

### Schemes

static let tokenType: NLTagScheme

A scheme that classifies tokens according to their broad type: word, punctuation, or whitespace.

static let lexicalClass: NLTagScheme

A scheme that classifies tokens according to class: part of speech, type of punctuation, or whitespace.

static let nameType: NLTagScheme

A scheme that classifies tokens according to whether they are part of a named entity.

static let nameTypeOrLexicalClass: NLTagScheme

A scheme that classifies tokens corresponding to names according to nameType, and classifies all other tokens according to lexicalClass.

static let lemma: NLTagScheme

A scheme that supplies a stem form of a word token, if known.

static let language: NLTagScheme

A scheme that supplies the language for a token, if it can determine one.

static let script: NLTagScheme

A scheme that supplies the script for a token, if it can determine one.

static let sentimentScore: NLTagScheme

A scheme that scores text as positive, negative, or neutral based on its sentiment polarity.

### Initializers

init(String)

Creates a tag scheme.

init(rawValue: String)

Creates a tag scheme with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the tag schemes

class func availableTagSchemes(for: NLTokenUnit, language: NLLanguage) -> [NLTagScheme]

Retrieves the tag schemes available for a particular unit (like word or sentence) and language on the current device.

class func requestAssets(for: NLLanguage, tagScheme: NLTagScheme, completionHandler: (NLTagger.AssetsResult, (any Error)?) -> Void)

Asks the Natural Language framework to load any missing assets for a tag scheme onto the device for the given language.

enum AssetsResult

The response to an asset request.

var tagSchemes: [NLTagScheme]

The tag schemes configured for this linguistic tagger.

