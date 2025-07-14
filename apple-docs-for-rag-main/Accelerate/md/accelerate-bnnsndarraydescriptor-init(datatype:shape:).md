

- Accelerate
- BNNSNDArrayDescriptor
-  init(dataType:shape:) 

Initializer

# init(dataType:shape:)

Returns a new n-dimensional array descriptor from the specified data type and shape.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
init(
    dataType: BNNSDataType,
    shape: BNNS.Shape
)
```

## Parameters 

`dataType`  

The data type of the data.

`shape`  

The shape of the n-dimensional array descriptor.

## See Also

### Creating an Array Descriptor

init(flags: BNNSNDArrayFlags, layout: BNNSDataLayout, size: (Int, Int, Int, Int, Int, Int, Int, Int), stride: (Int, Int, Int, Int, Int, Int, Int, Int), data: UnsafeMutableRawPointer?, data_type: BNNSDataType, table_data: UnsafeMutableRawPointer?, table_data_type: BNNSDataType, data_scale: Float, data_bias: Float)

Returns a new n-dimensional array descriptor with the specified parameters.

init?(data: UnsafeMutableRawBufferPointer, scalarType: any BNNSScalar.Type, shape: BNNS.Shape)

Returns a new n-dimensional array descriptor that references the same data as the specified raw pointer.

init?&lt;T>(data: UnsafeMutableBufferPointer&lt;T>, shape: BNNS.Shape)

Returns a new n-dimensional array descriptor that references the same data as the specified pointer.

init()

Returns a new n-dimensional array descriptor.

