

- Accelerate
- vImage_Buffer
-  size 

Instance Property

# size

The size of the image, in pixels.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
var size: CGSize { get }
```

## See Also

### Inspecting a buffer’s properties

var data: UnsafeMutableRawPointer!

A pointer to the top-left pixel of the image.

var height: vImagePixelCount

The height of the image, in pixels.

var width: vImagePixelCount

The width of the image, in pixels.

var rowBytes: Int

The distance, in bytes, between the start of one pixel row and the next in an image, including any unused space between them.

