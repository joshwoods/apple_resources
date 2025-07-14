

- Foundation
-  NSLinguisticTagScheme 

Structure

# NSLinguisticTagScheme

Constants for the tag schemes specified when initializing a linguistic tagger.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSLinguisticTagScheme
```

## Discussion

When initializing a linguistic tagger with init(tagSchemes:options:), you specify one or more tag schemes that correspond to the kind of information you’re interested in for a selection of natural language text. To ensure optimal performance, avoid specifying tag schemes that you won’t use.

Some tag schemes are only available for certain units and languages. Use the availableTagSchemes(for:language:) or availableTagSchemes(forLanguage:) methods to determine the possible values for a specified language and linguistic unit.

When working with linguistic tags using the methods described in Getting Linguistic Tags and Enumerating Linguistic Tags, the returned tag value depends on the specified scheme. For example, given the token “Überraschung”, the returned tag is noun when using the lexicalClass tag scheme, “de” (German language) when using the language tag scheme, and “Latn” (Latin script) when using the script tag scheme, as shown in the following code.

```
let tagger = NSLinguisticTagger(tagSchemes: [.lexicalClass, .language, .script], options: 0)
tagger.string = "Überraschung"

tagger.tag(at: 0, unit: .word, scheme: .lexicalClass, tokenRange: nil) // Noun
tagger.tag(at: 0, unit: .word, scheme: .language, tokenRange: nil) // de
tagger.tag(at: 0, unit: .word, scheme: .script, tokenRange: nil) // Latn
```

The following table lists the available tag schemes, their applicable linguistic units, and possible tag values.

| Linguistic tag scheme | Applicable linguistic units | Possible tag values |
|----|----|----|
| tokenType | NSLinguisticTaggerUnit.word | See Token Types |
| lexicalClass | NSLinguisticTaggerUnit.word | See Lexical Classes |
| nameType | NSLinguisticTaggerUnit.word | See Name Types |
| nameTypeOrLexicalClass | NSLinguisticTaggerUnit.word | See Name Types and Lexical Classes |
| lemma | NSLinguisticTaggerUnit.word | A stem of the word |
| language | NSLinguisticTaggerUnit.word, NSLinguisticTaggerUnit.sentence, NSLinguisticTaggerUnit.paragraph, NSLinguisticTaggerUnit.document | A BCP-47 language tag |
| script | NSLinguisticTaggerUnit.word, NSLinguisticTaggerUnit.sentence, NSLinguisticTaggerUnit.paragraph, NSLinguisticTaggerUnit.document | An ISO 15924 script code |

## Topics

### Schemes

static let tokenType: NSLinguisticTagScheme

Classifies tokens according to their broad type: word, punctuation, or whitespace.

Deprecated

static let lexicalClass: NSLinguisticTagScheme

Classifies tokens according to class: part of speech, type of punctuation, or whitespace.

Deprecated

static let nameType: NSLinguisticTagScheme

Classifies tokens according to whether they are part of a named entity.

Deprecated

static let nameTypeOrLexicalClass: NSLinguisticTagScheme

Classifies tokens corresponding to names according to nameType, and classifies all other tokens according to lexicalClass.

Deprecated

static let lemma: NSLinguisticTagScheme

Supplies a stem form of a word token, if known.

Deprecated

static let language: NSLinguisticTagScheme

Supplies the language for a token, if one can be determined.

Deprecated

static let script: NSLinguisticTagScheme

Supplies the script for a token, if one can be determined.

Deprecated

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Types

enum NSLinguisticTaggerUnit

Constants representing linguistic units.

struct NSLinguisticTag

A token, lexical class, name, lemma, language, or script returned by a linguistic tagger for natural language text.

