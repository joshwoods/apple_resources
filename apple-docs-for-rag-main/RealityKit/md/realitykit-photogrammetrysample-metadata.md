

- RealityKit
- PhotogrammetrySample
-  metadata 

Instance Property

# metadata

An image’s EXIF metadata.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var metadata: [String : Any] { get set }
```

## Discussion

You can provide EXIF metadata captured by your digital camera to assist in the object-creation process. During object creation, RealityKit can use data from the EXIF keys listed below.

- `TIFFMake`

- `TIFFModel`

- `TIFFOrientation`

- `ExifBodySerialNumber`

- `ExifLensMake`

- `ExifLensModel`

- `ExifLensSerialNumber`

- `ExifFocalLength`

- `ExifFocalLengthIn35mmFilm`

- `GPSAltitude`

- `GPSAltitudeRef`

- `GPSLatitude`

- `GPSLatitudeRef`

- `GPSLongitude`

- `GPSLongitudeRef`

## See Also

### Describing the sample

let image: CVPixelBuffer

The image data for this sample.

var depthDataMap: CVPixelBuffer?

The image’s depth data.

var gravity: CMAcceleration?

An image’s gravity vector.

var objectMask: CVPixelBuffer?

The image’s object mask.

