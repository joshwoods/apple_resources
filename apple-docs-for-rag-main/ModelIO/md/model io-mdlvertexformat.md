

- Model I/O
-  MDLVertexFormat 

Enumeration

# MDLVertexFormat

Descriptions of the data size and layout for a vertex attribute, used by the format property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLVertexFormat
```

## Overview

The values for vertex formats are constructed such that you can use bit masks to infer useful information about a format:

- The lowest order byte contains the number of vector components in a vertex format. For example, the raw value for the MDLVertexFormat.char3 format is the bitwise OR of the 3 (the number of components) with the MDLVertexFormat.charBits value.

- Special packed formats such as MDLVertexFormat.int1010102Normalized have values less than `0x10000`.

- For unpacked formats, masking away the lower four bytes leaves information about the data type for scalars or vector components.

## Topics

### Constants

case invalid

The vertex attribute has just been initialized or its format is unknown.

case packedBit

A bit mask for vertex attributes in packed vector formats.

case uCharBits

A bit mask for vertex attributes whose components are in 8-bit unsigned integer format.

case charBits

A bit mask for vertex attributes whose components are in 8-bit signed integer format.

case uCharNormalizedBits

A bit mask for vertex attributes whose components are in 8-bit unsigned normalized integer format.

case charNormalizedBits

A bit mask for vertex attributes whose components are in 8-bit signed normalized integer format.

case uShortBits

A bit mask for vertex attributes whose components are in 16-bit unsigned integer format.

case shortBits

A bit mask for vertex attributes whose components are in 16-bit signed integer format.

case uShortNormalizedBits

A bit mask for vertex attributes whose components are in 16-bit unsigned normalized integer format.

case shortNormalizedBits

A bit mask for vertex attributes whose components are in 16-bit signed normalized integer format.

case uIntBits

A bit mask for vertex attributes whose components are in 32-bit unsigned integer format.

case intBits

A bit mask for vertex attributes whose components are in 32-bit signed integer format.

case halfBits

A bit mask for vertex attributes whose components are in 16-bit floating-point format.

case floatBits

A bit mask for vertex attributes whose components are in 32-bit floating-point format.

case uChar

The attribute value for each vertex is a scalar of unsigned 8-bit integer type.

case uChar2

The attribute value for each vertex is a vector with 2 components, each of unsigned 8-bit integer type.

case uChar3

The attribute value for each vertex is a vector with 3 components, each of unsigned 8-bit integer type.

case uChar4

The attribute value for each vertex is a vector with 4 components, each of unsigned 8-bit integer type.

case char

The attribute value for each vertex is a scalar of signed 8-bit integer type.

case char2

The attribute value for each vertex is a vector with 2 components, each of signed 8-bit integer type.

case char3

The attribute value for each vertex is a vector with 3 components, each of signed 8-bit integer type.

case char4

The attribute value for each vertex is a vector with 4 components, each of signed 8-bit integer type.

case uCharNormalized

The attribute value for each vertex is a normalized scalar of unsigned 8-bit integer type.

case uChar2Normalized

The attribute value for each vertex is a vector with 2 components, each with a normalized value of unsigned 8-bit integer type.

case uChar3Normalized

The attribute value for each vertex is a vector with 3 components, each with a normalized value of unsigned 8-bit integer type.

case uChar4Normalized

The attribute value for each vertex is a vector with 4 components, each with a normalized value of unsigned 8-bit integer type.

case charNormalized

The attribute value for each vertex is a normalized scalar of signed 8-bit integer type.

case char2Normalized

The attribute value for each vertex is a vector with 2 components, each with a normalized value of signed 8-bit integer type.

case char3Normalized

The attribute value for each vertex is a vector with 3 components, each with a normalized value of signed 8-bit integer type.

case char4Normalized

The attribute value for each vertex is a vector with 4 components, each with a normalized value of signed 8-bit integer type.

case uShort

The attribute value for each vertex is a scalar of unsigned 16-bit integer type.

case uShort2

The attribute value for each vertex is a vector with 2 components, each of unsigned 16-bit integer type.

case uShort3

The attribute value for each vertex is a vector with 3 components, each of unsigned 16-bit integer type.

case uShort4

The attribute value for each vertex is a vector with 4 components, each of unsigned 16-bit integer type.

case short

The attribute value for each vertex is a scalar of signed 16-bit integer type.

case short2

The attribute value for each vertex is a vector with 2 components, each of signed 16-bit integer type.

case short3

The attribute value for each vertex is a vector with 3 components, each of signed 16-bit integer type.

case short4

The attribute value for each vertex is a vector with 4 components, each of signed 16-bit integer type.

case uShortNormalized

The attribute value for each vertex is a normalized scalar of unsigned 16-bit integer type.

case uShort2Normalized

The attribute value for each vertex is a vector with 2 components, each with a normalized value of unsigned 16-bit integer type.

case uShort3Normalized

The attribute value for each vertex is a vector with 3 components, each with a normalized value of unsigned 16-bit integer type.

case uShort4Normalized

The attribute value for each vertex is a vector with 4 components, each with a normalized value of unsigned 16-bit integer type.

case shortNormalized

The attribute value for each vertex is a normalized scalar of signed 16-bit integer type.

case short2Normalized

The attribute value for each vertex is a vector with 2 components, each with a normalized value of signed 16-bit integer type.

case short3Normalized

The attribute value for each vertex is a vector with 3 components, each with a normalized value of signed 16-bit integer type.

case short4Normalized

The attribute value for each vertex is a vector with 4 components, each with a normalized value of signed 16-bit integer type.

case uInt

The attribute value for each vertex is a scalar of unsigned 32-bit integer type.

case uInt2

The attribute value for each vertex is a vector with 2 components, each of unsigned 32-bit integer type.

case uInt3

The attribute value for each vertex is a vector with 3 components, each of unsigned 32-bit integer type.

case uInt4

The attribute value for each vertex is a vector with 4 components, each of unsigned 32-bit integer type.

case int

The attribute value for each vertex is a scalar of signed 32-bit integer type.

case int2

The attribute value for each vertex is a vector with 2 components, each of signed 32-bit integer type.

case int3

The attribute value for each vertex is a vector with 3 components, each of signed 32-bit integer type.

case int4

The attribute value for each vertex is a vector with 4 components, each of signed 32-bit integer type.

case half

The attribute value for each vertex is a scalar of 16-bit floating-point type.

case half2

The attribute value for each vertex is a vector with 2 components, each of 16-bit floating-point type.

case half3

The attribute value for each vertex is a vector with 3 components, each of 16-bit floating-point type.

case half4

The attribute value for each vertex is a vector with 4 components, each of 16-bit floating-point type.

case float

The attribute value for each vertex is a scalar of 32-bit floating-point type.

case float2

The attribute value for each vertex is a vector with 2 components, each of 32-bit floating-point type.

case float3

The attribute value for each vertex is a vector with 3 components, each of 32-bit floating-point type.

case float4

The attribute value for each vertex is a vector with 4 components, each of 32-bit floating-point type.

case int1010102Normalized

The attribute value for each vertex is a packed vector with 4 components of signed integer type. The first three components are 10 bits each, and the fourth component is 2 bits.

case uInt1010102Normalized

The attribute value for each vertex is a packed vector with 4 components of unsigned integer type. The first three components are 10 bits each, and the fourth component is 2 bits.

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

### Constants

Vertex Attributes

Names that identify semantic uses for vertex attribute data, used by the name property.

