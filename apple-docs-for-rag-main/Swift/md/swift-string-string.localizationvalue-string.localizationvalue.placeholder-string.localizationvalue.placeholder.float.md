

- Swift
- String
- String.LocalizationValue
- String.LocalizationValue.Placeholder
-  String.LocalizationValue.Placeholder.float 

Case

# String.LocalizationValue.Placeholder.float

The single-precision floating-point type, as used for replacement values with the localized string placeholder syntax.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
case float
```

## Discussion

To insert a `float` into a placeholder, use the syntax `\(placeholder: .float)`.

The various `String(localized:)` initializers apply a locale-appropriate `FormatStyle` to the numeric value, based on the `locale:` parameter or the `LocalizedStringResource`.

## See Also

### Placeholder types

case int

The signed integer type, as used for replacement values with the localized string placeholder syntax.

case uint

The unsigned integer type, as used for replacement values with the localized string placeholder syntax.

case double

The double-precision floating-point type, as used for replacement values with the localized string placeholder syntax.

case object

The object type, as used for replacement values with the localized string placeholder syntax.

