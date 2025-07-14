

- Accelerate
- vImage
- vImage.PixelBuffer
-  withUnsafeVImageBuffers(\_:) 

Instance Method

# withUnsafeVImageBuffers(\_:)

Calls the given closure with the underlying vImage buffers.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func withUnsafeVImageBuffers(_ body: ([vImage_Buffer]) throws -> R) rethrows -> R
```

Available when `Format` conforms to `MultiplePlanePixelFormat`.

## Parameters 

`body`  

A closure with a vImage_Buffer parameter that points to the underlying vImage buffers of the pixel buffer.

## Return Value

The return value, if any, of the body closure parameter.

## Discussion

Use this function to incorporate pixel buffer based image processing code with existing vImage code. For example, the following code accesses each multiple-plane pixel buffer’s underlying vImage buffers’ `rowBytes` property:

```
 let src = vImage.PixelBuffer(size: vImage.Size(width: 32,
                                                                 height: 64))

 src.withUnsafeVImageBuffers { vImageBuffers in
    for buffer in vImageBuffers {
        print(buffer.rowBytes)
     }
 }
```

## See Also

### Accessing underlying vImage buffers

func withUnsafePointerToVImageBuffer&lt;R>((UnsafePointer&lt;vImage_Buffer>) throws -> R) rethrows -> R

Calls the given closure with an unsafe pointer to the underlying vImage buffer.

func withUnsafeVImageBuffer&lt;R>((vImage_Buffer) throws -> R) rethrows -> R

Calls the given closure with the underlying vImage buffer.

