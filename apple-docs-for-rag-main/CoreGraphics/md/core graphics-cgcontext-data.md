

- Core Graphics
- CGContext
-  data 

Instance Property

# data

Returns a pointer to the image data associated with a bitmap context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var data: UnsafeMutableRawPointer? { get }
```

## Discussion

If you provided the memory for the bitmap data, you can use this method to get that data pointer. If you passed `NULL` for the data pointer when creating your bitmap context, it is safe to get the data pointer in iOS 4.0 and later and macOS 10.6 and later only. In earlier versions of the operating system, passing `NULL` for the data parameter is not supported and may lead to crashes when attempting to access this data using this function.

## See Also

### Managing a Bitmap Graphics Context

var bitmapInfo: CGBitmapInfo

Obtains the bitmap information associated with a bitmap graphics context.

var alphaInfo: CGImageAlphaInfo

Returns the alpha information associated with the context, which indicates how a bitmap context handles the alpha component.

var bitsPerComponent: Int

Returns the bits per component of a bitmap context.

var bitsPerPixel: Int

Returns the bits per pixel of a bitmap context.

var bytesPerRow: Int

Returns the bytes per row of a bitmap context.

var colorSpace: CGColorSpace?

Returns the color space of a bitmap context.

var height: Int

Returns the height in pixels of a bitmap context.

var width: Int

Returns the width in pixels of a bitmap context.

func makeImage() -> CGImage?

Creates and returns a CGImage from the pixel data in a bitmap graphics context.

