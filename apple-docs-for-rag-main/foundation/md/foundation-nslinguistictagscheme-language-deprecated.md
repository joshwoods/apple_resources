

- Foundation
- NSLinguisticTagScheme
-  language Deprecated

Type Property

# language

Supplies the language for a token, if one can be determined.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
static let language: NSLinguisticTagScheme
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Discussion

Each value for this tag scheme is a BCP-47 language identifier. For example, the language identifier for English is “en” and the identifier for Chinese written using the Simplified Chinese script is “zh-Hans”. The identifier “und” is used if a specific language cannot be determined.

The tagger generally attempts to determine the language of text at the level of an entire sentence, paragraph, or document, rather than word by word.

## See Also

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

static let script: NSLinguisticTagScheme

Supplies the script for a token, if one can be determined.

Deprecated

