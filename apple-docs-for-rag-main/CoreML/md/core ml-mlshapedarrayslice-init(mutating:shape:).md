

- Core ML
- MLShapedArraySlice
-  init(mutating:shape:) 

Initializer

# init(mutating:shape:)

Creates a new `MLShapedArraySlice` using a pixel buffer as the backing storage.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    mutating pixelBuffer: CVPixelBuffer,
    shape: [Int]
)
```

## Parameters 

`pixelBuffer`  

The pixel buffer to be owned by the instance.

`shape`  

The shape of the MLShapedArray. The last dimension of `shape` must match the pixel buffer’s width. The product of the rest of the dimensions must match the height.

## Discussion

Use this initializer to create an IOSurface backed `MLShapedArraySlice`, which can reduce the inference latency by avoiding the buffer copy.

The pixel buffer’s pixel format type must be `OneComponent16Half`. As such, the scalar type must be `Float16`.

```
var pixelBuffer: CVPixelBuffer?
let pixelBufferAttributes = [
    kCVPixelBufferIOSurfacePropertiesKey : [:]
]
// Pixel buffer's width is the last dimension of `shape`, which is 4.
// The height is the product of the rest of the dimensions, which is
// 2 * 3 = 6.
CVPixelBufferCreate(kCFAllocatorDefault,
                    4, 6,
                    kCVPixelFormatType_OneComponent16Half,
                    pixelBufferAttributes as CFDictionary,
                    &pixelBuffer)

let shapedArray = MLShapedArraySlice(mutating: pixelBuffer!,
                                              shape: [2, 3, 4])
```

When there is one and only one owner of the shaped array, mutating operations modifies the underlying pixel buffer.

```
var slice = MLShapedArraySlice(mutating: pixelBuffer, shape: [1])
slice[scalarAt: 0] = 42
// The pixel buffer now has 42 in its frame buffer.
```

It follows the value semantics. The mutation doesn’t affect the copy.

```
var slice1 = MLShapedArraySlice(mutating: pixelBuffer, shape: [1])
slice1[scalarAt: 0] = 0 // pixelBuffer is mutated.
let slice2 = slice1
slice1[scalarAt: 0] = 42 // Copy-on-Write

assert(slice1[scalarAt: 0] == 42)
assert(slice2[scalarAt: 0] == 0)
```

