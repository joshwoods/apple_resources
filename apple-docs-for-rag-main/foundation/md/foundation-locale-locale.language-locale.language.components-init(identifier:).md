

- Foundation
- Locale
- Locale.Language
- Locale.Language.Components
-  init(identifier:) 

Initializer

# init(identifier:)

Creates a language components instance from a language identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(identifier: String)
```

## Parameters 

`identifier`  

A Unicode language identifier, like `en-US`, `es-419`, or `zh-Hant-TW`.

## See Also

### Creating a language components instance

init(language: Locale.Language)

Creates a language components instance from an existing language instance.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, region: Locale.Region?)

Creates a language components instance from a given language code, script, and region.

