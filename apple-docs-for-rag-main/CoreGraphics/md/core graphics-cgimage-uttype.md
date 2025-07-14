

- Core Graphics
- CGImage
-  utType 

Instance Property

# utType

The Universal Type Identifier for the image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var utType: CFString? { get }
```

## See Also

### Examining an Image

var isMask: Bool

Returns whether a bitmap image is an image mask.

var width: Int

Returns the width of a bitmap image, in pixels.

var height: Int

Returns the height of a bitmap image.

var bitsPerComponent: Int

Returns the number of bits allocated for a single color component of a bitmap image.

var bitsPerPixel: Int

Returns the number of bits allocated for a single pixel in a bitmap image.

var bytesPerRow: Int

Returns the number of bytes allocated for a single row of a bitmap image.

var colorSpace: CGColorSpace?

Return the color space for a bitmap image.

var alphaInfo: CGImageAlphaInfo

Returns the alpha channel information for a bitmap image.

enum CGImageAlphaInfo

Storage options for alpha component data.

var dataProvider: CGDataProvider?

Returns the data provider for a bitmap image or image mask.

var decode: UnsafePointer&lt;CGFloat>?

Returns the decode array for a bitmap image.

var shouldInterpolate: Bool

Returns the interpolation setting for a bitmap image.

var renderingIntent: CGColorRenderingIntent

Returns the rendering intent setting for a bitmap image.

var bitmapInfo: CGBitmapInfo

Returns the bitmap information for a bitmap image.

struct CGBitmapInfo

Component information for a bitmap image.

