

- Metal
-  MTLVertexFormat 

Enumeration

# MTLVertexFormat

Values that specify the organization of function vertex data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLVertexFormat
```

## Topics

### Constants

case invalid

An invalid vertex format.

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

Two unsigned normalized 16-bit values.

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

case half

One half-precision floating-point value.

case half2

Two half-precision floating-point values.

case half3

Three half-precision floating-point values.

case half4

Four half-precision floating-point values.

case float

One single-precision floating-point value.

case float2

Two single-precision floating-point values.

case float3

Three single-precision floating-point values.

case float4

Four single-precision floating-point values.

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

case uchar4Normalized_bgra

Four unsigned normalized 8-bit values, arranged as blue, green, red, and alpha components.

### Enumeration Cases

case floatRG11B10

case floatRGB9E5

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

