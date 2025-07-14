

- Foundation
- Locale
-  init(components:) 

Initializer

# init(components:)

Creates a locale from the given components.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(components: Locale.Components)
```

## Parameters 

`components`  

A Locale.Components instance that provides the components to create a customized locale.

## Discussion

Use this initializer to create a locale with a unique combination of components, beyond the defaults provided by a language and country code.

For example, you can create a Locale.Components instance that uses UK language conventions, but US regional conventions for traits like currency and measurement. You then use the components to create a new Locale instance, like this:

```
var components = Locale.Components(languageCode: "en", languageRegion: "GB")
components.region = Locale.Region("US")
let en_GB_US = Locale(components: components)
```

## See Also

### Creating a locale by components

struct Components

A type that represents the components of a locale, for use when creating a locale with specific overrides.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, languageRegion: Locale.Region?)

Creates a locale with the specified language code, script, and region identifier.

init(languageComponents: Locale.Language.Components)

Creates a locale from the given language components.

struct Components

A type that identifies a language by its various components.

