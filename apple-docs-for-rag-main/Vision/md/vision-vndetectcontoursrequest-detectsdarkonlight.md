

- Vision
- VNDetectContoursRequest
-  detectsDarkOnLight 

Instance Property

# detectsDarkOnLight

A Boolean value that indicates whether the request detects a dark object on a light background to aid in detection.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var detectsDarkOnLight: Bool { get set }
```

## Discussion

The default value is true.

## See Also

### Configuring the Request

var contrastAdjustment: Float

The amount by which to adjust the image contrast.

var contrastPivot: NSNumber?

The pixel value to use as a pivot for the contrast.

var maximumImageDimension: Int

The maximum image dimension to use for contour detection.

var detectDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background.

Deprecated

