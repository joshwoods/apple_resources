

- Core Spotlight
- CSSearchableItemAttributeSet
-  acquisitionModel 

Instance Property

# acquisitionModel

The model of the device that captured the image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var acquisitionModel: String? { get set }
```

## See Also

### Describing images

var isoSpeed: NSNumber?

The ISO speed setting at the time the camera captured the image.

var acquisitionMake: String?

The manufacturer of the device that captured the image.

var aperture: NSNumber?

The size of the lens aperture at the time the camera captured the image, as a log-scale APEX value.

var bitsPerSample: NSNumber?

The number of bits per sample.

var cameraOwner: String?

The owner of the camera that captured the image.

var colorSpace: String?

The color space model the image uses, such as RGB, CMYK, YUV, or YCbCr.

var flashOn: NSNumber?

A value that indicates if the camera used a flash to capture the image.

var focalLength: NSNumber?

The actual focal length of the lens, in millimeters.

var focalLength35mm: NSNumber?

A value that indicates if the focal length is 35mm.

var layerNames: [String]?

An array that contains the names of the various layers in the file.

var lensModel: String?

The model of the lens that captured the image.

var orientation: NSNumber?

The orientation of the data.

var pixelCount: NSNumber?

The total number of pixels in the image.

var pixelHeight: NSNumber?

The height of the item, such as image or video frame height, in pixels.

var pixelWidth: NSNumber?

The width of the item, such as image or video frame width, in pixels.

