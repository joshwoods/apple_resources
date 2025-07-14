

- Foundation
- Locale
- Locale.Language
- Locale.Language.Components
-  init(language:) 

Initializer

# init(language:)

Creates a language components instance from an existing language instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(language: Locale.Language)
```

## Parameters 

`language`  

A Locale.Language instance. This initializer copies over the language code, script, and region from the provided language.

## See Also

### Creating a language components instance

init(identifier: String)

Creates a language components instance from a language identifier.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, region: Locale.Region?)

Creates a language components instance from a given language code, script, and region.

