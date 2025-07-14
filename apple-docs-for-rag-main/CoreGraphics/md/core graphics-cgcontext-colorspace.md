

- Core Graphics
- CGContext
-  colorSpace 

Instance Property

# colorSpace

Returns the color space of a bitmap context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var colorSpace: CGColorSpace? { get }
```

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

var data: UnsafeMutableRawPointer?

Returns a pointer to the image data associated with a bitmap context.

var height: Int

Returns the height in pixels of a bitmap context.

var width: Int

Returns the width in pixels of a bitmap context.

func makeImage() -> CGImage?

Creates and returns a CGImage from the pixel data in a bitmap graphics context.

