

- Accelerate
- vImage
- vImage.PixelBuffer
-  withUnsafePointerToVImageBuffer(\_:) 

Instance Method

# withUnsafePointerToVImageBuffer(\_:)

Calls the given closure with an unsafe pointer to the underlying vImage buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func withUnsafePointerToVImageBuffer(_ body: (UnsafePointer) throws -> R) rethrows -> R
```

Available when `Format` conforms to `SinglePlanePixelFormat`.

## Parameters 

`body`  

A closure with an unsafe pointer to a vImage_Buffer parameter that points to the underlying vImage buffer of the pixel buffer.

## Return Value

The return value, if any, of the body closure parameter.

## Discussion

Use this function to incorporate pixel buffer based image processing code with existing vImage code. For example, the following code passes a pixel buffer to the C API vImageBufferFill_ARGB8888(_:_:_:) routine:

```
 let src = vImage.PixelBuffer(size: vImage.Size(width: 128, height: 128))

 src.withUnsafePointerToVImageBuffer { vImageBufferPtr in
     _ = vImageBufferFill_ARGB8888(vImageBufferPtr,
                                   [0, 0, 0, 0],
                                   vImage_Flags(kvImageNoFlags))
 }
```

## See Also

### Accessing underlying vImage buffers

func withUnsafeVImageBuffer&lt;R>((vImage_Buffer) throws -> R) rethrows -> R

Calls the given closure with the underlying vImage buffer.

func withUnsafeVImageBuffers&lt;R>(([vImage_Buffer]) throws -> R) rethrows -> R

Calls the given closure with the underlying vImage buffers.

