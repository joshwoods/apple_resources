

- Accelerate
- BNNS
- BNNS.Shape
-  layout 

Instance Property

# layout

The data layout of the shape.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
var layout: BNNSDataLayout { get }
```

## See Also

### Inspecting the Properties of a Shape

var batchStride: Int

The number of elements between each batch of data in the shape.

var rank: Int

The number of dimensions of the shape.

var size: (Int, Int, Int, Int, Int, Int, Int, Int)

The size, in elements, of each dimension of the shape.

var stride: (Int, Int, Int, Int, Int, Int, Int, Int)

The stride, in elements, of each dimension of the shape.

