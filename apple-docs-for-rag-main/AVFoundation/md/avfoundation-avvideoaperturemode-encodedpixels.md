

- AVFoundation
- AVVideoApertureMode
-  encodedPixels 

Type Property

# encodedPixels

The encoded dimensions of the image description are displayed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let encodedPixels: AVVideoApertureMode
```

## Discussion

The image is not cropped to the clean aperture region and is not scaled according to the pixel aspect ratio.

## See Also

### Aperture Modes

static let cleanAperture: AVVideoApertureMode

The pixel aspect ratio and clean aperture will be applied.

static let productionAperture: AVVideoApertureMode

The pixel aspect ratio will be applied.

