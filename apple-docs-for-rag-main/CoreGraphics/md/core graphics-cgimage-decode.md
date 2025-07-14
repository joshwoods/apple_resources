

- Core Graphics
- CGImage
-  decode 

Instance Property

# decode

Returns the decode array for a bitmap image.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var decode: UnsafePointer? { get }
```

## Discussion

For a bitmap image or image mask, for each color component in the source color space, the decode array contains a pair of values denoting the upper and lower limits of a range. When the image is rendered, a linear transform maps the original component value into a relative number, within the designated range, that is appropriate for the destination color space. If remapping of the image’s color values is not allowed, the returned value will be `NULL`.

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

var shouldInterpolate: Bool

Returns the interpolation setting for a bitmap image.

var renderingIntent: CGColorRenderingIntent

Returns the rendering intent setting for a bitmap image.

var bitmapInfo: CGBitmapInfo

Returns the bitmap information for a bitmap image.

struct CGBitmapInfo

Component information for a bitmap image.

var utType: CFString?

The Universal Type Identifier for the image.

