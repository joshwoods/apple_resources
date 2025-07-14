

- Swift
- String
-  String.LocalizationValue 

Structure

# String.LocalizationValue

A reference to a localizable string, with optional string interpolation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct LocalizationValue
```

## Overview

Use this type when the localization key is the localized string value in the development language. This type also supports creating localized strings that depend on a value you provide at runtime. For example, if your app’s strings catalog contains a localizable entry for `"Hello, \(userName)."`, you create a localized string like the following:

```
    let greeting = String(localized: "Hello, \(userName).")
```

If you want to use an arbitary string as your localization key, use String initializers that take a StaticString and a `defaultValue` parameter, like init(localized:defaultValue:table:bundle:locale:comment:) and init(localized:defaultValue:options:table:bundle:locale:comment:).

If you need to provide localized strings to another process that might be using a different locale, initialize with a `LocalizedStringResource`, using init(localized:) or init(localized:options:).

## Topics

### Creating a string localization value instance

init(String)

Creates a localization value instance.

### Supporting types

enum Placeholder

An enumeration of types that can appear as a placeholder in a string interpolation.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Sendable

## See Also

### Creating a Localized String

init(localized: String.LocalizationValue, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an interpolated string.

init(localized: String.LocalizationValue, options: String.LocalizationOptions, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an interpolated string, applying the specified options.

struct LocalizationOptions

Options to apply when initializing a localized string.

init(localized: StaticString, defaultValue: String.LocalizationValue, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an arbitrary static string key.

init(localized: StaticString, defaultValue: String.LocalizationValue, options: String.LocalizationOptions, table: String?, bundle: Bundle?, locale: Locale, comment: StaticString?)

Creates a localized string from an arbitrary static string key, applying the specified options.

init(localized: LocalizedStringResource)

Creates a localized string from a localized string resource.

init(localized: LocalizedStringResource, options: String.LocalizationOptions)

Creates a localized string from a localized string resource, applying the specified options.

