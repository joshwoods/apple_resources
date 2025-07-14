

- Swift
- String
- String.LocalizationValue
-  String.LocalizationValue.Placeholder 

Enumeration

# String.LocalizationValue.Placeholder

An enumeration of types that can appear as a placeholder in a string interpolation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Placeholder
```

## Overview

Foundation uses this type when you create a string with the `\(placeholder: type)` syntax and supply an array of replacement values in a `String.LocalizationOptions`. Placeholders work with String initializers that take an `options:` parameter:

- init(localized:options:table:bundle:locale:comment:)

- init(localized:options:)

- init(localized:defaultValue:options:table:bundle:locale:comment:)

You only use this type directly when specifying one of its enumeration cases in the placeholder syntax, like `\(placeholder: .int)`.

## Topics

### Placeholder types

case int

The signed integer type, as used for replacement values with the localized string placeholder syntax.

case uint

The unsigned integer type, as used for replacement values with the localized string placeholder syntax.

case float

The single-precision floating-point type, as used for replacement values with the localized string placeholder syntax.

case double

The double-precision floating-point type, as used for replacement values with the localized string placeholder syntax.

case object

The object type, as used for replacement values with the localized string placeholder syntax.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

