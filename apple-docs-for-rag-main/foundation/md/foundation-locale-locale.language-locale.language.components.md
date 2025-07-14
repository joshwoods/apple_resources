

- Foundation
- Locale
- Locale.Language
-  Locale.Language.Components 

Structure

# Locale.Language.Components

A type that identifies a language by its various components.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Components
```

## Topics

### Creating a language components instance

init(identifier: String)

Creates a language components instance from a language identifier.

init(language: Locale.Language)

Creates a language components instance from an existing language instance.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, region: Locale.Region?)

Creates a language components instance from a given language code, script, and region.

### Examining language component properties

var languageCode: Locale.LanguageCode?

The language code that identifies this language.

struct LanguageCode

An alphabetical code associated with a language.

var region: Locale.Region?

The region used with this language.

struct Region

A type that represents a geographic region, for use in specifying a locale or language.

var script: Locale.Script?

The written script used by this language.

struct Script

The written script used with a given language.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a locale by components

init(components: Locale.Components)

Creates a locale from the given components.

struct Components

A type that represents the components of a locale, for use when creating a locale with specific overrides.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, languageRegion: Locale.Region?)

Creates a locale with the specified language code, script, and region identifier.

init(languageComponents: Locale.Language.Components)

Creates a locale from the given language components.

