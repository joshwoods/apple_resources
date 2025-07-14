

- Metal
-  MTLDataType 

Enumeration

# MTLDataType

The types of GPU functions, including shaders and compute kernels.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLDataType
```

## Topics

### Boolean Types

case bool

A Boolean value.

case bool2

A two-component Boolean vector.

case bool3

A three-component Boolean vector.

case bool4

A four-component Boolean vector.

### 8-bit Integer Types

case char

An 8-bit, signed integer value.

case char2

A two-component vector with 8-bit, signed integer values.

case char3

A three-component vector with 8-bit, signed integer values.

case char4

A four-component vector with 8-bit, signed integer values.

case uchar

An 8-bit, unsigned integer value.

case uchar2

A two-component vector with 8-bit, unsigned integer values.

case uchar3

A three-component vector with 8-bit, unsigned integer values.

case uchar4

A four-component vector with 8-bit, unsigned integer values.

### 16-bit Integer Types

case short

A 16-bit, signed integer value.

case short2

A two-component vector with 16-bit, signed integer values.

case short3

A three-component vector with 16-bit, signed integer values.

case short4

A four-component vector with 16-bit, signed integer values.

case ushort

A 16-bit, unsigned integer value.

case ushort2

A two-component vector with 16-bit, unsigned integer values.

case ushort3

A three-component vector with 16-bit, unsigned integer values.

case ushort4

A four-component vector with 16-bit, unsigned integer values.

### 16-bit Floating-Point Types

case half

A 16-bit floating-point value.

case half2

A two-component vector with 16-bit floating-point values.

case half3

A three-component vector with 16-bit floating-point values.

case half4

A four-component vector with 16-bit floating-point values.

case half2x2

A 2x2 component matrix with 16-bit floating-point values.

case half2x3

A 2x3 component matrix with 16-bit floating-point values.

case half2x4

A 2x4 component matrix with 16-bit floating-point values.

case half3x2

A 3x2 component matrix with 16-bit floating-point values.

case half3x3

A 3x3 component matrix with 16-bit floating-point values.

case half3x4

A 3x4 component matrix with 16-bit floating-point values.

case half4x2

A 4x2 component matrix with 16-bit floating-point values.

case half4x3

A 4x3 component matrix with 16-bit floating-point values.

case half4x4

A 4x4 component matrix with 16-bit floating-point values.

case bfloat

A 16-bit, brain floating-point value.

case bfloat2

A two-component vector with 16-bit, brain floating-point values.

case bfloat3

A three-component vector with 16-bit, brain floating-point values.

case bfloat4

A four-component vector with 16-bit, brain floating-point values.

### 32-bit Floating-Point Types

case float

A 32-bit floating-point value.

case float2

A two-component vector with 32-bit floating-point values.

case float3

A three-component vector with 32-bit floating-point values.

case float4

A four-component vector with 32-bit floating-point values.

case float2x2

A 2x2 component matrix with 32-bit floating-point values.

case float2x3

A 2x3 component matrix with 32-bit floating-point values.

case float2x4

A 2x4 component matrix with 32-bit floating-point values.

case float3x2

A 3x2 component matrix with 32-bit floating-point values.

case float3x3

A 3x3 component matrix with 32-bit floating-point values.

case float3x4

A 3x4 component matrix with 32-bit floating-point values.

case float4x2

A 4x2 component matrix with 32-bit floating-point values.

case float4x3

A 4x3 component matrix with 32-bit floating-point values.

case float4x4

A 4x4 component matrix with 32-bit floating-point values.

### 32-bit Integer Types

case int

A 32-bit, signed integer value.

case int2

A two-component vector with 32-bit, signed integer values.

case int3

A three-component vector with 32-bit, signed integer values.

case int4

A four-component vector with 32-bit, signed integer values.

case uint

A 32-bit, unsigned integer value.

case uint2

A two-component vector with 32-bit, unsigned integer values.

case uint3

A three-component vector with 32-bit, unsigned integer values.

case uint4

A four-component vector with 32-bit, unsigned integer values.

### 64-bit Integer Types

case long

A 64-bit, signed integer value.

case long2

A two-component vector with 64-bit, signed integer values.

case long3

A three-component vector with 64-bit, signed integer values.

case long4

A four-component vector with 64-bit, signed integer values.

case ulong

A 64-bit, unsigned integer value.

case ulong2

A two-component vector with 64-bit, unsigned integer values.

case ulong3

A three-component vector with 64-bit, unsigned integer values.

case ulong4

A four-component vector with 64-bit, unsigned integer values.

### 8-bit Pixel Format Types

case r8Snorm

An ordinary pixel with one component that’s an 8-bit, normalized, signed integer value.

case r8Unorm

An ordinary pixel with one component that’s an 8-bit, normalized, unsigned integer value.

### 16-bit Pixel Format Types

case rg8Snorm

An ordinary pixel with two components, each of which is an 8-bit, normalized, signed integer value.

case rg8Unorm

An ordinary pixel with two components, each of which is an 8-bit, normalized, unsigned integer value.

case r16Snorm

An ordinary pixel with one component that’s a 16-bit, normalized, signed integer value.

case r16Unorm

An ordinary pixel with one component that’s a 16-bit, normalized, unsigned integer value.

### 32-bit Pixel Format Types

case rgba8Snorm

An ordinary pixel with four components, each of which is an 8-bit, normalized, signed integer value.

case rgba8Unorm

An ordinary pixel with four components, each of which is an 8-bit, normalized, unsigned integer value.

case rgba8Unorm_srgb

An ordinary pixel with four components, each of which is an 8-bit, normalized, unsigned integer value in the sRGB color space.

case rg16Snorm

An ordinary pixel with two components, each of which is a 16-bit, normalized, signed integer value.

case rg16Unorm

An ordinary pixel with two components, each of which is a 16-bit, normalized, unsigned integer value.

case rgb10a2Unorm

A packed 32-bit format with three color components, each of which is a 10-bit, normalized, unsigned integer value.

case rgb9e5Float

A packed 32-bit format with three color components, each of which is a 9-bit floating-point value.

case rg11b10Float

A packed 32-bit format with three floating-point color components, two of which are 11-bit values, and one is a 10-bit value.

### 64-bit Pixel Format Types

case rgba16Snorm

An ordinary pixel with four components, each of which is a 16-bit, normalized, signed integer value.

case rgba16Unorm

An ordinary pixel with four components, each of which is a 16-bit, normalized, unsigned integer value.

### Metal Resource Types

case texture

A Metal texture resource instance.

case indirectCommandBuffer

An indirect command buffer resource instance.

case visibleFunctionTable

A table of visible functions that a render or compute pipeline can call.

case intersectionFunctionTable

A table of intersection functions that a render or compute pipeline can call.

case primitiveAccelerationStructure

A low-level ray-tracing acceleration structure for a set of primitives.

case instanceAccelerationStructure

A high-level, ray-tracing acceleration structure for a set of low-level primitive instances.

### Metal State Types

case sampler

A Metal texture sampler instance.

case renderPipeline

A Metal render pipeline instance.

case computePipeline

A Metal compute pipeline instance.

### Collection Types

case `struct`

A structure instance.

case array

An array instance.

case pointer

A pointer.

### Invalid Data Types

case none

A placeholder that represents a GPU function parameter that doesn’t have a valid data type.

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

### Shader Types

class MTLType

A description of a data type.

class MTLArrayType

A description of an array.

class MTLStructType

A description of a structure.

class MTLStructMember

An object that provides information about a field in a structure.

class MTLPointerType

A description of a pointer.

class MTLTextureReferenceType

A description of a texture.

