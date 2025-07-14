

- Foundation
- FormatStyle
-  number 

Type Property

# number

A style for formatting 32-bit unsigned integers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var number: IntegerFormatStyle { get }
```

Available when `Self` is `IntegerFormatStyle`.

## Discussion

Use this type property when the call point allows the use of IntegerFormatStyle. You typically do this when calling the `formatted` methods of types that conform to BinaryInteger.

## See Also

### Applying numeric styles for integers

static var number: IntegerFormatStyle&lt;Int>

A style for formatting the Swift default integer type.

static var number: IntegerFormatStyle&lt;UInt>

A style for formatting the Swift unsigned integer type.

static var number: IntegerFormatStyle&lt;Int8>

A style for formatting 8-bit signed integers.

static var number: IntegerFormatStyle&lt;Int16>

A style for formatting 16-bit signed integers.

static var number: IntegerFormatStyle&lt;Int32>

A style for formatting 32-bit signed integers.

static var number: IntegerFormatStyle&lt;Int64>

A style for formatting 64-bit signed integers.

static var number: IntegerFormatStyle&lt;UInt8>

A style for formatting 8-bit unsigned integers.

static var number: IntegerFormatStyle&lt;UInt16>

A style for formatting 16-bit unsigned integers.

static var number: IntegerFormatStyle&lt;UInt64>

A style for formatting 64-bit unsigned integers.

struct IntegerFormatStyle

A structure that converts between integer values and their textual representations.

