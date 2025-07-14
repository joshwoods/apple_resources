

- Core Foundation
-  CFNumberType 

Enumeration

# CFNumberType

Flags used by CFNumber to indicate the data type of a value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFNumberType
```

## Overview

The type specified in the call to CFNumberCreate(_:_:_:) is not necessarily preserved when creating a new CFNumber object. A CFNumber object uses whatever internal storage type the creation function deems appropriate. Use the CFNumberGetType(_:) function to find out what type the CFNumber object used to store your value.

## Topics

### Constants

case sInt8Type

Eight-bit, signed integer. The `SInt8` data type is defined in `MacTypes.h`.

case sInt16Type

Sixteen-bit, signed integer. The `SInt16` data type is defined in `MacTypes.h`.

case sInt32Type

Thirty-two-bit, signed integer. The `SInt32` data type is defined in `MacTypes.h`.

case sInt64Type

Sixty-four-bit, signed integer. The `SInt64` data type is defined in `MacTypes.h`.

case float32Type

Thirty-two-bit real. The `Float32` data type is defined in `MacTypes.h`.

case float64Type

Sixty-four-bit real. The `Float64` data type is defined in `MacTypes.h` and conforms to the 64-bit IEEE 754 standard.

case charType

Basic C `char` type.

case shortType

Basic C `short` type.

case intType

Basic C `int` type.

case longType

Basic C `long` type.

case longLongType

Basic C `long long` type.

case floatType

Basic C `float` type.

case doubleType

Basic C `double` type.

case cfIndexType

CFIndex value.

case nsIntegerType

`NSInteger` value.

case cgFloatType

`CGFloat` value.

static var maxType: CFNumberType

Same as CFNumberType.cgFloatType.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Predefined Values

CFNumber provides some predefined number values.

