

- Foundation
- Locale
-  Locale.Script 

Structure

# Locale.Script

The written script used with a given language.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Script
```

## Topics

### Creating a script

init(String)

Creates a script from a BCP 47 identifier.

### Examining script properties

var identifier: String

### Using defined scripts

static let unknown: Locale.Script

### Instance Properties

var isISOScript: Bool

### Type Properties

static var adlam: Locale.Script

static var arabic: Locale.Script

static var arabicNastaliq: Locale.Script

static var armenian: Locale.Script

static var bangla: Locale.Script

static var cherokee: Locale.Script

static var cyrillic: Locale.Script

static var devanagari: Locale.Script

static var ethiopic: Locale.Script

static var georgian: Locale.Script

static var greek: Locale.Script

static var gujarati: Locale.Script

static var gurmukhi: Locale.Script

static var hanSimplified: Locale.Script

static var hanTraditional: Locale.Script

static var hanifiRohingya: Locale.Script

static var hebrew: Locale.Script

static var hiragana: Locale.Script

static var japanese: Locale.Script

static var kannada: Locale.Script

static var katakana: Locale.Script

static var khmer: Locale.Script

static var korean: Locale.Script

static var lao: Locale.Script

static var latin: Locale.Script

static var malayalam: Locale.Script

static var meiteiMayek: Locale.Script

static var myanmar: Locale.Script

static var odia: Locale.Script

static var olChiki: Locale.Script

static var sinhala: Locale.Script

static var syriac: Locale.Script

static var tamil: Locale.Script

static var telugu: Locale.Script

static var thaana: Locale.Script

static var thai: Locale.Script

static var tibetan: Locale.Script

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

struct LanguageCode

An alphabetical code associated with a language.

var region: Locale.Region?

The region used with the language.

struct Region

A type that represents a geographic region, for use in specifying a locale or language.

var script: Locale.Script?

The written script of the language.

var characterDirection: Locale.LanguageDirection

The ordering of characters within a line.

typealias LanguageDirection

An alias for the standard set of language directions.

