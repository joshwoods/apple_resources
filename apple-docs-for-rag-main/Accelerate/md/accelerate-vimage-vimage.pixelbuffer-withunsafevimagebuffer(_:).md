

- Accelerate
- vImage
- vImage.PixelBuffer
-  withUnsafeVImageBuffer(\_:) 

Instance Method

# withUnsafeVImageBuffer(\_:)

Calls the given closure with the underlying vImage buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func withUnsafeVImageBuffer(_ body: (vImage_Buffer) throws -> R) rethrows -> R
```

Available when `Format` conforms to `SinglePlanePixelFormat`.

## Parameters 

`body`  

A closure with a vImage_Buffer parameter that points to the underlying vImage buffer of the pixel buffer.

## Return Value

The return value, if any, of the body closure parameter.

## Discussion

Use this function to incorporate pixel buffer based image processing code with existing vImage code. For example, the following code accesses a pixel buffer’s underlying vImage buffer’s `rowBytes` property:

```
 let src = try vImage.PixelBuffer(cgImage: cgImage,
                                                         cgImageFormat: &cgImageFormat)

 src.withUnsafeVImageBuffer { vImageBuffer in
     print(vImageBuffer.rowBytes)
 }
```

## See Also

### Accessing underlying vImage buffers

func withUnsafePointerToVImageBuffer&lt;R>((UnsafePointer&lt;vImage_Buffer>) throws -> R) rethrows -> R

Calls the given closure with an unsafe pointer to the underlying vImage buffer.

func withUnsafeVImageBuffers&lt;R>(([vImage_Buffer]) throws -> R) rethrows -> R

Calls the given closure with the underlying vImage buffers.

