

- Accelerate
-  BNNSLayerData Deprecated

Structure

# BNNSLayerData

A structure containing common layer parameters.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
struct BNNSLayerData
```

Deprecated

Use BNNSNDArrayDescriptor instead.

## Topics

### Initializers

init()

init(data: UnsafeRawPointer?, data_type: BNNSDataType, data_scale: Float, data_bias: Float, data_table: UnsafePointer&lt;Float>?)

Returns a new layer data structure.

init(data: UnsafeRawPointer?, data_type: BNNSDataType, data_scale: Float, data_bias: Float)

### Instance Properties

var data: UnsafeRawPointer?

Pointer to layer values (weights, bias), layout and size are specific to each layer.

var data_bias: Float

Conversion bias for values, used for integer data types only, ignored for indexed and float data types.

var data_scale: Float

Conversion scale for values, used for integer data types only, ignored for indexed and float data types.

var data_table: UnsafePointer&lt;Float>?

Conversion table (256 values) for indexed floating point data, used for indexed data types only.

var data_type: BNNSDataType

Storage data type for the values stored in data.

### Type Properties

static var zero: BNNSLayerData

### Type Methods

static func indexed8(data: UnsafePointer&lt;Int8>?, data_table: UnsafePointer&lt;Float>) -> BNNSLayerData

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### N-dimensional array descriptor essentials

enum Shape

Constants that describe the size and data layout of an n-dimensional array descriptor.

struct BNNSDataLayout

Constants that describe the data type of an n-dimensional array.

struct BNNSDataType

BNNS Data Types.

struct BNNSNDArrayDescriptor

A structure that describes the shape, stride, data type, and, optionally, the memory location of an n-dimensional array.

func BNNSDataLayoutGetRank(BNNSDataLayout) -> Int

