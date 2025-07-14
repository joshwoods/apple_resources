

- Foundation
- FormatStyle
-  percent 

Type Property

# percent

A style for formatting 16-bit floating-point values as a percent representation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var percent: FloatingPointFormatStyle.Percent { get }
```

Available when `Self` is `FloatingPointFormatStyle.Percent`.

## Discussion

Use this type property when the call point allows the use of FloatingPointFormatStyle. You typically do this when calling the `formatted` methods of types that conform to BinaryFloatingPoint.

## See Also

### Applying percentage styles for floating-point values

static var percent: FloatingPointFormatStyle&lt;Float>.Percent

A style for formatting the Swift standard single-precision floating-point type as a percent representation.

static var percent: FloatingPointFormatStyle&lt;Double>.Percent

A style for formatting the Swift standard single-precision floating-point type as a percent representation.

struct Percent

A format style that converts between floating-point percentage values and their textual representations.

