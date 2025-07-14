

- Foundation
- Locale
- Locale.Components
-  init(identifier:) 

Initializer

# init(identifier:)

Creates a locale components instance with the specified identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(identifier: String)
```

## Parameters 

`identifier`  

A BCP-47 language identifier such as `en-u-nu-thai-ca-buddhist` or an ICU-style identifier such as `en@calendar=buddhist;numbers=thai`.

## See Also

### Creating a locale components instance

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, languageRegion: Locale.Region?)

Creates a locale components instance with the specified language code, script, and region identifier.

init(locale: Locale)

Creates a language components instance from an existing locale.

