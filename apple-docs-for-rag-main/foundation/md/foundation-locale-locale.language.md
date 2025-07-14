

- Foundation
- Locale
-  Locale.Language 

Structure

# Locale.Language

A type that represents a language, as used in a locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Language
```

## Topics

### Creating a language

init(identifier: String)

Creates a language from an identifier.

init(components: Locale.Language.Components)

Creates a language from its component values.

struct Components

A type that identifies a language by its various components.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, region: Locale.Region?)

Creates a language from a given language code, script, and region.

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

struct Script

The written script used with a given language.

var characterDirection: Locale.LanguageDirection

The ordering of characters within a line.

typealias LanguageDirection

An alias for the standard set of language directions.

### Examining language relationships

var parent: Locale.Language?

The parent language of this language, if available.

func hasCommonParent(with: Locale.Language) -> Bool

Returns a Boolean value that indicates if the given language shares a common parent with this language.

func isEquivalent(to: Locale.Language) -> Bool

Returns a Boolean value that indicates whether this language and another language are equivalent after expanding missing components.

### Using system languages

static var systemLanguages: [Locale.Language]

An array of the system’s supported languages.

### Instance Properties

var lineLayoutDirection: Locale.LanguageDirection

var maximalIdentifier: String

var minimalIdentifier: String

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Getting language components

var language: Locale.Language

The language of a locale.

