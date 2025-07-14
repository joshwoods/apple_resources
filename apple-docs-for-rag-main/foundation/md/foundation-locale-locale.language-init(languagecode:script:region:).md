

- Foundation
- Locale
- Locale.Language
-  init(languageCode:script:region:) 

Initializer

# init(languageCode:script:region:)

Creates a language from a given language code, script, and region.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    languageCode: Locale.LanguageCode? = nil,
    script: Locale.Script? = nil,
    region: Locale.Region? = nil
)
```

## Parameters 

`languageCode`  

A language code, typically created from a two- or three-letter language code specified by ISO 639.

`script`  

The script to use for the new locale components instance.

`region`  

The region to use for the new components instance.

## See Also

### Creating a language

init(identifier: String)

Creates a language from an identifier.

init(components: Locale.Language.Components)

Creates a language from its component values.

struct Components

A type that identifies a language by its various components.

