

- Foundation
- Locale
-  Locale.LanguageCode 

Structure

# Locale.LanguageCode

An alphabetical code associated with a language.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct LanguageCode
```

## Topics

### Creating a language code

init(String)

Creates a language code from an identifier.

### Examining language code properties

var identifier: String

The identifier used to create the language code.

var isISOLanguage: Bool

A Boolean value that indicates whether this language code is in the list of ISO-defined languages.

### Using ISO-defined language codes

static var isoLanguageCodes: [Locale.LanguageCode]

Returns an array of ISO-defined language codes.

### Instance Methods

func identifier(Locale.LanguageCode.IdentifierType) -> String?

### Type Properties

static var ainu: Locale.LanguageCode

static var albanian: Locale.LanguageCode

static var amharic: Locale.LanguageCode

static var apacheWestern: Locale.LanguageCode

static var arabic: Locale.LanguageCode

static var armenian: Locale.LanguageCode

static var assamese: Locale.LanguageCode

static var assyrian: Locale.LanguageCode

static var azerbaijani: Locale.LanguageCode

static var bangla: Locale.LanguageCode

static var belarusian: Locale.LanguageCode

static var bodo: Locale.LanguageCode

static var bulgarian: Locale.LanguageCode

static var burmese: Locale.LanguageCode

static var cantonese: Locale.LanguageCode

static var catalan: Locale.LanguageCode

static var cherokee: Locale.LanguageCode

static var chinese: Locale.LanguageCode

static var croatian: Locale.LanguageCode

static var czech: Locale.LanguageCode

static var danish: Locale.LanguageCode

static var dhivehi: Locale.LanguageCode

static var dogri: Locale.LanguageCode

static var dutch: Locale.LanguageCode

static var dzongkha: Locale.LanguageCode

static var english: Locale.LanguageCode

static var estonian: Locale.LanguageCode

static var faroese: Locale.LanguageCode

static var finnish: Locale.LanguageCode

static var french: Locale.LanguageCode

static var fula: Locale.LanguageCode

static var georgian: Locale.LanguageCode

static var german: Locale.LanguageCode

static var greek: Locale.LanguageCode

static var gujarati: Locale.LanguageCode

static var hawaiian: Locale.LanguageCode

static var hebrew: Locale.LanguageCode

static var hindi: Locale.LanguageCode

static var hungarian: Locale.LanguageCode

static var icelandic: Locale.LanguageCode

static var igbo: Locale.LanguageCode

static var indonesian: Locale.LanguageCode

static var irish: Locale.LanguageCode

static var italian: Locale.LanguageCode

static var japanese: Locale.LanguageCode

static var kannada: Locale.LanguageCode

static var kashmiri: Locale.LanguageCode

static var kazakh: Locale.LanguageCode

static var khmer: Locale.LanguageCode

static var konkani: Locale.LanguageCode

static var korean: Locale.LanguageCode

static var kurdish: Locale.LanguageCode

static var kurdishSorani: Locale.LanguageCode

static var kyrgyz: Locale.LanguageCode

static var lao: Locale.LanguageCode

static var latvian: Locale.LanguageCode

static var lithuanian: Locale.LanguageCode

static var māori: Locale.LanguageCode

static var macedonian: Locale.LanguageCode

static var maithili: Locale.LanguageCode

static var malay: Locale.LanguageCode

static var malayalam: Locale.LanguageCode

static var maltese: Locale.LanguageCode

static var manipuri: Locale.LanguageCode

static var marathi: Locale.LanguageCode

static var mongolian: Locale.LanguageCode

static let multiple: Locale.LanguageCode

static var navajo: Locale.LanguageCode

static var nepali: Locale.LanguageCode

static var norwegian: Locale.LanguageCode

static var norwegianBokmål: Locale.LanguageCode

static var norwegianNynorsk: Locale.LanguageCode

static var odia: Locale.LanguageCode

static var pashto: Locale.LanguageCode

static var persian: Locale.LanguageCode

static var polish: Locale.LanguageCode

static var portuguese: Locale.LanguageCode

static var punjabi: Locale.LanguageCode

static var rohingya: Locale.LanguageCode

static var romanian: Locale.LanguageCode

static var russian: Locale.LanguageCode

static var samoan: Locale.LanguageCode

static var sanskrit: Locale.LanguageCode

static var santali: Locale.LanguageCode

static var serbian: Locale.LanguageCode

static var sindhi: Locale.LanguageCode

static var sinhala: Locale.LanguageCode

static var slovak: Locale.LanguageCode

static var slovenian: Locale.LanguageCode

static var spanish: Locale.LanguageCode

static var swahili: Locale.LanguageCode

static var swedish: Locale.LanguageCode

static var tagalog: Locale.LanguageCode

static var tajik: Locale.LanguageCode

static var tamil: Locale.LanguageCode

static var telugu: Locale.LanguageCode

static var thai: Locale.LanguageCode

static var tibetan: Locale.LanguageCode

static var tongan: Locale.LanguageCode

static var turkish: Locale.LanguageCode

static var turkmen: Locale.LanguageCode

static var ukrainian: Locale.LanguageCode

static let unavailable: Locale.LanguageCode

static let uncoded: Locale.LanguageCode

static let unidentified: Locale.LanguageCode

static var urdu: Locale.LanguageCode

static var uyghur: Locale.LanguageCode

static var uzbek: Locale.LanguageCode

static var vietnamese: Locale.LanguageCode

static var welsh: Locale.LanguageCode

static var yiddish: Locale.LanguageCode

### Enumerations

enum IdentifierType

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- Sendable

## See Also

### Examining language properties

var languageCode: Locale.LanguageCode?

The language code that identifies the language.

var region: Locale.Region?

The region used with the language.

struct Region

A type that represents a geographic region, for use in specifying a locale or language.

var script: Locale.Script?

The written script of the language.

struct Script

The written script used with a given language.

var characterDirection: Locale.LanguageDirection

The ordering of characters within a line.

typealias LanguageDirection

An alias for the standard set of language directions.

