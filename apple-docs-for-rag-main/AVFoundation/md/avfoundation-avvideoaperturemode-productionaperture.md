

- AVFoundation
- AVVideoApertureMode
-  productionAperture 

Type Property

# productionAperture

The pixel aspect ratio will be applied.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let productionAperture: AVVideoApertureMode
```

## Discussion

The image is not cropped to the clean aperture region, but it is scaled according to the pixel aspect ratio. Use this option when you want to see all the pixels in your video, including the edges.

## See Also

### Aperture Modes

static let cleanAperture: AVVideoApertureMode

The pixel aspect ratio and clean aperture will be applied.

static let encodedPixels: AVVideoApertureMode

The encoded dimensions of the image description are displayed.

