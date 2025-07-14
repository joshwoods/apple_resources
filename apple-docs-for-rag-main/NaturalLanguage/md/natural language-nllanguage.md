

- Natural Language
-  NLLanguage 

Structure

# NLLanguage

The languages that the Natural Language framework supports.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct NLLanguage
```

## Mentioned in 

Identifying the language in text

## Topics

### Getting standard languages

static let amharic: NLLanguage

The unique identifier string for the Amharic language.

static let arabic: NLLanguage

The unique identifier string for the Arabic language.

static let armenian: NLLanguage

The unique identifier string for the Armenian language.

static let bengali: NLLanguage

The unique identifier string for the Bengali language.

static let bulgarian: NLLanguage

The unique identifier string for the Bulgarian language.

static let burmese: NLLanguage

The unique identifier string for the Burmese language.

static let catalan: NLLanguage

The unique identifier string for the Catalan language.

static let cherokee: NLLanguage

The unique identifier string for the Cherokee language.

static let croatian: NLLanguage

The unique identifier string for the Croatian language.

static let czech: NLLanguage

The unique identifier string for the Czech language.

static let danish: NLLanguage

The unique identifier string for the Danish language.

static let dutch: NLLanguage

The unique identifier string for the Dutch language.

static let english: NLLanguage

The unique identifier string for the English language.

static let finnish: NLLanguage

The unique identifier string for the Finnish language.

static let french: NLLanguage

The unique identifier string for the French language.

static let georgian: NLLanguage

The unique identifier string for the Georgian language.

static let german: NLLanguage

The unique identifier string for the German language.

static let greek: NLLanguage

The unique identifier string for the Greek language.

static let gujarati: NLLanguage

The unique identifier string for the Gujarati language.

static let hebrew: NLLanguage

The unique identifier string for the Hebrew language.

static let hindi: NLLanguage

The unique identifier string for the Hindi language.

static let hungarian: NLLanguage

The unique identifier string for the Hungarian language.

static let icelandic: NLLanguage

The unique identifier string for the Icelandic language.

static let indonesian: NLLanguage

The unique identifier string for the Indonesian language.

static let italian: NLLanguage

The unique identifier string for the Italian language.

static let japanese: NLLanguage

The unique identifier string for the Japanese language.

static let kannada: NLLanguage

The unique identifier string for the Kannada language.

static let kazakh: NLLanguage

The unique identifier string for the Kazakh language.

static let khmer: NLLanguage

The unique identifier string for the Khmer language.

static let korean: NLLanguage

The unique identifier string for the Korean language.

static let lao: NLLanguage

The unique identifier string for the Lao language.

static let malay: NLLanguage

The unique identifier string for the Malay language.

static let malayalam: NLLanguage

The unique identifier string for the Malayalam language.

static let marathi: NLLanguage

The unique identifier string for the Marathi language.

static let mongolian: NLLanguage

The unique identifier string for the Mongolian language.

static let norwegian: NLLanguage

The unique identifier string for the Norwegian language.

static let oriya: NLLanguage

The unique identifier string for the Oriya language.

static let persian: NLLanguage

The unique identifier string for the Persian language.

static let polish: NLLanguage

The unique identifier string for the Polish language.

static let portuguese: NLLanguage

The unique identifier string for the Portuguese language.

static let punjabi: NLLanguage

The unique identifier string for the Punjabi language.

static let romanian: NLLanguage

The unique identifier string for the Romanian language.

static let russian: NLLanguage

The unique identifier string for the Russian language.

static let simplifiedChinese: NLLanguage

The unique identifier string for the Simplified Chinese language.

static let sinhalese: NLLanguage

The unique identifier string for the Sinhalese language.

static let slovak: NLLanguage

The unique identifier string for the Slovak language.

static let spanish: NLLanguage

The unique identifier string for the Spanish language.

static let swedish: NLLanguage

The unique identifier string for the Swedish language.

static let tamil: NLLanguage

The unique identifier string for the Tamil language.

static let telugu: NLLanguage

The unique identifier string for the Telugu language.

static let thai: NLLanguage

The unique identifier string for the Thai language.

static let tibetan: NLLanguage

The unique identifier string for the Tibetan language.

static let traditionalChinese: NLLanguage

The unique identifier string for the Traditional Chinese language.

static let turkish: NLLanguage

The unique identifier string for the Turkish language.

static let ukrainian: NLLanguage

The unique identifier string for the Ukrainian language.

static let urdu: NLLanguage

The unique identifier string for the Urdu language.

static let vietnamese: NLLanguage

The unique identifier string for the Vietnamese language.

static let undetermined: NLLanguage

The unique identifier string for a language the Natural Language framework doesn’t recognize.

### Creating custom language tags

init(String)

Creates a language tag with the given string.

init(rawValue: String)

Creates a language tag with the given string as its raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Language identification

Identifying the language in text

Detect the language in a piece of text by using a language recognizer.

class NLLanguageRecognizer

The language of a body of text.

