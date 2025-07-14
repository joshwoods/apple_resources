

- Accelerate
- vImage
- vImage.PixelBuffer
-  withUnsafeBufferPointer(\_:) 

Instance Method

# withUnsafeBufferPointer(\_:)

Calls the given closure with a pointer to the buffer’s contiguous storage.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func withUnsafeBufferPointer(_ body: (UnsafeBufferPointer) throws -> R) rethrows -> R
```

Available when `Format` conforms to `StaticPixelFormat`.

## Parameters 

`body`  

A closure with an UnsafeBufferPointer parameter that points to the contiguous storage for the pixel buffer.

## Return Value

The return value, if any, of the body closure parameter.

## Discussion

You can use this function to simplify interoperation with other libraries and frameworks. For example, the following code uses Accelerate’s vForce library to raise each pixel value to the power of `1 / 2.2`:

```
let srcBuffer = vImage.PixelBuffer(pixelValues: [0.1, 0.2, 0.3, 0.4],
                                   size: vImage.Size(width: 4, height: 1),
                                   pixelFormat: vImage.PlanarF.self)

let destBuffer =  vImage.PixelBuffer(size: srcBuffer.size,
                                     pixelFormat: vImage.PlanarF.self)

var exponent = Float(1 / 2.2)
var count = Int32(4)

srcBuffer.withUnsafeBufferPointer { src in
    destBuffer.withUnsafeMutableBufferPointer { dest in

        vvpowsf(dest.baseAddress!,
                &exponent,
                src.baseAddress!,
                &count)
    }
}
```

Note

The contiguous storage may include space outside of the buffer’s width that doesn’t contain image information. The storage contains `rowStride * channelCount * height` elements.

