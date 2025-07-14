

- Metal
-  MTLAttributeFormat 

Enumeration

# MTLAttributeFormat

Values indicating the organization and format of data for function attributes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
enum MTLAttributeFormat
```

## Overview

All data formats are least significant bit first (little-endian). For compute functions which manipulate data consumed by other parts of your app, ensure that the data exposed to the GPU is byte- and bit-aligned correctly to the source format. Your compute function’s attributes can be of a different type than the original source data, so long as they use the same number of bits. For example, your compute function can interpret a 128-bit little-endian integer as MTLAttributeFormat.uint4.

Note

When manipulating pixel data in a compute function for a future pipeline stage, use an exact match for the underlying pixel data to avoid visual corruption.

## Topics

### Invalid format

case invalid

An invalid format.

### Character data formats

case uchar

One unsigned 8-bit value.

case uchar2

Two unsigned 8-bit values.

case uchar3

Three unsigned 8-bit values.

case uchar4

Four unsigned 8-bit values.

case char

One signed 8-bit two’s complement value.

case char2

Two signed 8-bit two’s complement values.

case char3

Three signed 8-bit two’s complement values.

case char4

Four signed 8-bit two’s complement values.

case ucharNormalized

One unsigned normalized 8-bit value.

case uchar2Normalized

Two unsigned normalized 8-bit values.

case uchar3Normalized

Three unsigned normalized 8-bit values.

case uchar4Normalized

Four unsigned normalized 8-bit values.

case charNormalized

One signed normalized 8-bit two’s complement value.

case char2Normalized

Two signed normalized 8-bit two’s complement values.

case char3Normalized

Three signed normalized 8-bit two’s complement values.

case char4Normalized

Four signed normalized 8-bit two’s complement values.

### 16- bit integer data formats

case ushort

One unsigned 16-bit value.

case ushort2

Two unsigned 16-bit values.

case ushort3

Three unsigned 16-bit values.

case ushort4

Four unsigned 16-bit values.

case short

One signed 16-bit two’s complement value.

case short2

Two signed 16-bit two’s complement values.

case short3

Three signed 16-bit two’s complement values.

case short4

Four signed 16-bit two’s complement values.

case ushortNormalized

One unsigned normalized 16-bit value.

case ushort2Normalized

Two unsigned normalized 16-bit values

case ushort3Normalized

Three unsigned normalized 16-bit values.

case ushort4Normalized

Four unsigned normalized 16-bit values.

case shortNormalized

One signed normalized 16-bit two’s complement value.

case short2Normalized

Two signed normalized 16-bit two’s complement values.

case short3Normalized

Three signed normalized 16-bit two’s complement values.

case short4Normalized

Four signed normalized 16-bit two’s complement values.

### 32-bit integer data formats

case uint

One unsigned 32-bit value.

case uint2

Two unsigned 32-bit values.

case uint3

Three unsigned 32-bit values.

case uint4

Four unsigned 32-bit values.

case int

One signed 32-bit two’s complement value.

case int2

Two signed 32-bit two’s complement values.

case int3

Three signed 32-bit two’s complement values.

case int4

Four signed 32-bit two’s complement values.

case int1010102Normalized

One packed 32-bit value with four normalized signed two’s complement integer values, arranged as 10 bits, 10 bits, 10 bits, and 2 bits.

case uint1010102Normalized

One packed 32-bit value with four normalized unsigned integer values, arranged as 10 bits, 10 bits, 10 bits, and 2 bits.

### 16-bit floating point formats

case half

One half-precision floating-point value.

case half2

Two half-precision floating-point values.

case half3

Three half-precision floating-point values.

case half4

Four half-precision floating-point values.

### 32-bit floating point formats

case float

One single-precision floating-point value.

case float2

Two single-precision floating-point values.

case float3

Three single-precision floating-point values.

case float4

Four single-precision floating-point values.

### Pixel data types

case uchar4Normalized_bgra

Four unsigned normalized 8-bit values, arranged as blue, green, red, and alpha components.

case floatRG11B10

One packed 32-bit value representing pixel data containing 11-bit float red and green channels, and a 10-bit float blue channel.

case floatRGB9E5

One packed 32-bit value representing pixel data containing 9-bit float red, green, and blue channels, and a 5-bit float shared exponent channel.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Defining Attribute Location

var bufferIndex: Int

The index in the buffer argument table for the buffer that contains the data for this attribute.

var offset: Int

The offset, in bytes, from the start of the buffer containing the attribute data to the start of the data itself.

var format: MTLAttributeFormat

The format of the attribute’s data.

