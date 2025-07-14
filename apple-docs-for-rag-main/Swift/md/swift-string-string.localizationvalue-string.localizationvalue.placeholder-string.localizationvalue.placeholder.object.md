

- Swift
- String
- String.LocalizationValue
- String.LocalizationValue.Placeholder
-  String.LocalizationValue.Placeholder.object 

Case

# String.LocalizationValue.Placeholder.object

The object type, as used for replacement values with the localized string placeholder syntax.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
case object
```

## Discussion

To insert a object into a placeholder, use the syntax `\(placeholder: .object)`.

String.LocalizationValue supports interpolating `NSObject` instances and Foundation types that bridge to `NSObject` types.

## See Also

### Placeholder types

case int

The signed integer type, as used for replacement values with the localized string placeholder syntax.

case uint

The unsigned integer type, as used for replacement values with the localized string placeholder syntax.

case float

The single-precision floating-point type, as used for replacement values with the localized string placeholder syntax.

case double

The double-precision floating-point type, as used for replacement values with the localized string placeholder syntax.

