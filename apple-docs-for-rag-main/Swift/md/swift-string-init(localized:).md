

- Swift
- String
-  init(localized:) 

Initializer

# init(localized:)

Creates a localized string from a localized string resource.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(localized resource: LocalizedStringResource)
```

## Parameters 

`resource`  

A `LocalizedStringResource` that provides the localization key, table, bundle, and locale.

## Discussion

Call this initializer to look up the localization that `resource` indicates from a string catalog or `strings` file in your app bundle. Alter the resource’s `locale` prior to calling this method if you want to localize this string in a different locale than the process that creates the `LocalizedStringResource`.

```
// Assume the string catalog contains "Hello, world!" for English
// and "Bonjour, le monde!" for French.
var localizable = LocalizedStringResource("Hello, world!")
// Potentially using localizable in another process…
localizable.locale = Locale(identifier: "en")
let enLocalized = String(localized: localizable)
localizable.locale = Locale(identifier: "fr")
let frLocalized = String(localized: localizable)
// enLocalized == "Hello, world!"
// frLocalized == "Bonjour, le monde!"
```

If you don’t need the deferred-loading behavior of `LocalizedStringResource`, use init(localized:table:bundle:locale:comment:) instead. If you prefer to use an arbitrary localization key rather than the localized string in the development language, use init(localized:defaultValue:table:bundle:locale:comment:).

## See Also

### Creating a Localized String

init(localized: String.LocalizationValue, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an interpolated string.

init(localized: String.LocalizationValue, options: String.LocalizationOptions, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an interpolated string, applying the specified options.

struct LocalizationValue

A reference to a localizable string, with optional string interpolation.

struct LocalizationOptions

Options to apply when initializing a localized string.

init(localized: StaticString, defaultValue: String.LocalizationValue, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an arbitrary static string key.

init(localized: StaticString, defaultValue: String.LocalizationValue, options: String.LocalizationOptions, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an arbitrary static string key, applying the specified options.

init(localized: LocalizedStringResource, options: String.LocalizationOptions)

Creates a localized string from a localized string resource, applying the specified options.

