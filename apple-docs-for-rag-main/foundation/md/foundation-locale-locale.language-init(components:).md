

- Foundation
- Locale
- Locale.Language
-  init(components:) 

Initializer

# init(components:)

Creates a language from its component values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(components: Locale.Language.Components)
```

## Parameters 

`components`  

A Locale.Language.Components instance that provides a custom language code, region, and script for the new Locale.Language instance.

## See Also

### Creating a language

init(identifier: String)

Creates a language from an identifier.

struct Components

A type that identifies a language by its various components.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, region: Locale.Region?)

Creates a language from a given language code, script, and region.

