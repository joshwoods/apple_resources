

- Foundation
- Locale
- Locale.Components
-  init(languageCode:script:languageRegion:) 

Initializer

# init(languageCode:script:languageRegion:)

Creates a locale components instance with the specified language code, script, and region identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    languageCode: Locale.LanguageCode? = nil,
    script: Locale.Script? = nil,
    languageRegion: Locale.Region? = nil
)
```

## Parameters 

`languageCode`  

A language code, typically created from a two- or three-letter language code specified by ISO 639.

`script`  

The script to use for the new locale components instance.

`languageRegion`  

A language region, typically created from a two-letter BCP 47 region subtag like `US`.

## See Also

### Creating a locale components instance

init(identifier: String)

Creates a locale components instance with the specified identifier.

init(locale: Locale)

Creates a language components instance from an existing locale.

