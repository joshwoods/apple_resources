

- Foundation
- Locale
- Locale.Language
-  characterDirection 

Instance Property

# characterDirection

The ordering of characters within a line.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var characterDirection: Locale.LanguageDirection { get }
```

## Discussion

For example, English uses left-to-right while Mongolian in the Mongolian script uses top-to-bottom.

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

struct Script

The written script used with a given language.

typealias LanguageDirection

An alias for the standard set of language directions.

