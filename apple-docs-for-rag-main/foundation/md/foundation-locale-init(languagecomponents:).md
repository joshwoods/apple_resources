

- Foundation
- Locale
-  init(languageComponents:) 

Initializer

# init(languageComponents:)

Creates a locale from the given language components.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(languageComponents: Locale.Language.Components)
```

## Parameters 

`languageComponents`  

A Locale.Language.Components instance that provides language components that identify a locale.

## See Also

### Creating a locale by components

init(components: Locale.Components)

Creates a locale from the given components.

struct Components

A type that represents the components of a locale, for use when creating a locale with specific overrides.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, languageRegion: Locale.Region?)

Creates a locale with the specified language code, script, and region identifier.

struct Components

A type that identifies a language by its various components.

