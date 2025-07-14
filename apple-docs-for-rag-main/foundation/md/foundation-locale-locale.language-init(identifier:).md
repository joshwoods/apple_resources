

- Foundation
- Locale
- Locale.Language
-  init(identifier:) 

Initializer

# init(identifier:)

Creates a language from an identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(identifier: String)
```

## Parameters 

`identifier`  

A Unicode language identifier, like `en-US`, `es-419`, or `zh-Hant-TW`.

## See Also

### Creating a language

init(components: Locale.Language.Components)

Creates a language from its component values.

struct Components

A type that identifies a language by its various components.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, region: Locale.Region?)

Creates a language from a given language code, script, and region.

