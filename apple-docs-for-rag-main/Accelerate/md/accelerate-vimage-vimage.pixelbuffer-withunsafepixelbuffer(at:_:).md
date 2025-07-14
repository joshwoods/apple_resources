

- Accelerate
- vImage
- vImage.PixelBuffer
-  withUnsafePixelBuffer(at:\_:) 

Instance Method

# withUnsafePixelBuffer(at:\_:)

Calls the given closure with the pixel buffer that references the individual plane at the given index.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func withUnsafePixelBuffer(
    at index: Int,
    _ body: (vImage.PixelBuffer) throws -> R
) rethrows -> R
```

Available when `Format` conforms to `MultiplePlanePixelFormat`.

## Parameters 

`index`  

The index of the plane.

`body`  

A closure with a vImage.PixelBuffer parameter that points to the underlying pixel buffer at the given index.

## Return Value

The return value, if any, of the body closure parameter.

## Discussion

Use this function to access a single planar pixel buffer from a multiple-plane pixel buffer. For example, the following code converts the 8-bit pixels at plane `2` to 32-bit and writes the result to `dest`:

```
 let src = vImage.PixelBuffer(size: vImage.Size(width: 32,
                                                                  height: 64))

 let dest = vImage.PixelBuffer(size: src.size)

 src.withUnsafePixelBuffer(at: 2) { vImageBuffer in

     vImageBuffer.convert(to: dest)
 }
```

## See Also

### Accessing component pixel buffers

func withUnsafePixelBuffers&lt;R>(([vImage.PixelBuffer&lt;Format.PlanarPixelFormat>]) throws -> R) rethrows -> R

Calls the given closure with the array of pixel buffers that reference the individual planes.

