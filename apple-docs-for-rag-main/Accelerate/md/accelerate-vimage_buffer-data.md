

- Accelerate
- vImage_Buffer
-  data 

Instance Property

# data

A pointer to the top-left pixel of the image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var data: UnsafeMutableRawPointer!
```

## See Also

### Inspecting a buffer’s properties

var height: vImagePixelCount

The height of the image, in pixels.

var width: vImagePixelCount

The width of the image, in pixels.

var size: CGSize

The size of the image, in pixels.

var rowBytes: Int

The distance, in bytes, between the start of one pixel row and the next in an image, including any unused space between them.

