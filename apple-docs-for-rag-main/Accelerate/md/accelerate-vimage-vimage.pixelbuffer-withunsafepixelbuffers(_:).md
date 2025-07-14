

- Accelerate
- vImage
- vImage.PixelBuffer
-  withUnsafePixelBuffers(\_:) 

Instance Method

# withUnsafePixelBuffers(\_:)

Calls the given closure with the array of pixel buffers that reference the individual planes.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func withUnsafePixelBuffers(_ body: ([vImage.PixelBuffer]) throws -> R) rethrows -> R
```

Available when `Format` conforms to `MultiplePlanePixelFormat`.

## Parameters 

`body`  

A closure with an array vImage.PixelBuffer parameter that points to the underlying pixel buffers.

## Return Value

The return value, if any, of the body closure parameter.

## Discussion

Use this function to access each individual planar pixel buffer of a multiple-plane pixel buffer. For example, the following code initializes a 4-channel interleaved pixel buffer from the first three pixel buffers of a 4-channel multiple-plane pixel buffer:

```
 let src = vImage.PixelBuffer(size: vImage.Size(width: 32,
                                                                  height: 64))

 src.withUnsafePixelBuffers { overlaySource8x4PixelBuffers in

     let dest = vImage.PixelBuffer(planarBuffers: [
         overlaySource8x4PixelBuffers[0],
         overlaySource8x4PixelBuffers[1],
         overlaySource8x4PixelBuffers[2]
     ])
 }
```

## See Also

### Accessing component pixel buffers

func withUnsafePixelBuffer&lt;R>(at: Int, (vImage.PixelBuffer&lt;Format.PlanarPixelFormat>) throws -> R) rethrows -> R

Calls the given closure with the pixel buffer that references the individual plane at the given index.

