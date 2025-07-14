

- Swift
- String
-  String.LocalizationOptions 

Structure

# String.LocalizationOptions

Options to apply when initializing a localized string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct LocalizationOptions
```

## Overview

Use this type to configure how the system localizes strings. You can use the replacements property to provide replacement values for localizable strings that use the `\(placeholder:)` syntax.

## Topics

### Specifying localization behavior

var replacements: [any CVarArg]?

An array of replacement options.

### Initializers

init()

## See Also

### Creating a Localized String

init(localized: String.LocalizationValue, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an interpolated string.

init(localized: String.LocalizationValue, options: String.LocalizationOptions, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an interpolated string, applying the specified options.

struct LocalizationValue

A reference to a localizable string, with optional string interpolation.

init(localized: StaticString, defaultValue: String.LocalizationValue, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an arbitrary static string key.

init(localized: StaticString, defaultValue: String.LocalizationValue, options: String.LocalizationOptions, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an arbitrary static string key, applying the specified options.

init(localized: LocalizedStringResource)

Creates a localized string from a localized string resource.

init(localized: LocalizedStringResource, options: String.LocalizationOptions)

Creates a localized string from a localized string resource, applying the specified options.

