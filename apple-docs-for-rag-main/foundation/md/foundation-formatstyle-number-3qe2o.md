

- Foundation
- FormatStyle
-  number 

Type Property

# number

A style for formatting 16-bit floating-point values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var number: FloatingPointFormatStyle { get }
```

Available when `Self` is `FloatingPointFormatStyle`.

## Discussion

Use this type property when the call point allows the use of FloatingPointFormatStyle. You typically do this when calling the `formatted` methods of types that conform to BinaryFloatingPoint.

## See Also

### Applying numeric styles for floating-point values

static var number: FloatingPointFormatStyle&lt;Float>

A style for formatting the Swift standard single-precision floating-point type.

static var number: FloatingPointFormatStyle&lt;Double>

A style for formatting the Swift standard double-precision floating-point type.

struct FloatingPointFormatStyle

A structure that converts between floating-point values and their textual representations.

