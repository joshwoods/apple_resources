

- Foundation
- FormatStyle
-  percent 

Type Property

# percent

A style for formatting 8-bit unsigned integers as a percent representation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var percent: IntegerFormatStyle.Percent { get }
```

Available when `Self` is `IntegerFormatStyle.Percent`.

## Discussion

Use this type property when the call point allows the use of IntegerFormatStyle. You typically do this when calling the `formatted` methods of types that conform to BinaryInteger.

## See Also

### Applying percentage styles for integers

static var percent: IntegerFormatStyle&lt;Int>.Percent

A style for formatting signed integer types in Swift as a percent representation.

static var percent: IntegerFormatStyle&lt;UInt>.Percent

A style for formatting signed integer types in Swift as a percent representation.

static var percent: IntegerFormatStyle&lt;Int8>.Percent

A style for formatting 8-bit signed integers as a percent representation.

static var percent: IntegerFormatStyle&lt;Int16>.Percent

A style for formatting 16-bit signed integers as a percent representation.

static var percent: IntegerFormatStyle&lt;Int32>.Percent

A style for formatting 32-bit signed integers as a percent representation.

static var percent: IntegerFormatStyle&lt;Int64>.Percent

A style for formatting 64-bit signed integers as a percent representation.

static var percent: IntegerFormatStyle&lt;UInt16>.Percent

A style for formatting 16-bit unsigned integers as a percent representation.

static var percent: IntegerFormatStyle&lt;UInt32>.Percent

A style for formatting 32-bit unsigned integers as a percent representation.

static var percent: IntegerFormatStyle&lt;UInt64>.Percent

A style for formatting 64-bit unsigned integers as a percent representation.

struct Percent

A format style that converts between integer percentage values and their textual representations.

