

- Accelerate
- vImage
- vImage.PixelBuffer
-  applyMorphology(operation:destination:) 

Instance Method

# applyMorphology(operation:destination:)

Applies a morphology operation to the buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func applyMorphology(
    operation: vImage.MorphologyOperation,
    destination: vImage.PixelBuffer
)
```

Available when `Format` conforms to `MultiplePlanePixelFormat`, `Format.ComponentType` is `Float`, and `Format.PlanarPixelFormat.ComponentType` is `Float`.

## Parameters 

`operation`  

The operation that the function applies.

`destination`  

The destination pixel buffer.

## Discussion

Precondition

Source and destination buffer must be the same size.

Precondition

The kernel size width and height must be positive, odd integers in the range

Precondition

`dilate` and `erode` user defined kernels must contain `width * height` elements.

Precondition

Source and destination buffers must point to different underlying memory.

