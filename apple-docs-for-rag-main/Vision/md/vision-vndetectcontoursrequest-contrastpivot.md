

- Vision
- VNDetectContoursRequest
-  contrastPivot 

Instance Property

# contrastPivot

The pixel value to use as a pivot for the contrast.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var contrastPivot: NSNumber? { get set }
```

## Discussion

Numeric values range from `0.0` to `1.0`. You can also specify `nil` to have the framework automatically detect the value according to image intensity.

The default value is `0.5`, which indicates the pixel center.

## See Also

### Configuring the Request

var contrastAdjustment: Float

The amount by which to adjust the image contrast.

var detectsDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background to aid in detection.

var maximumImageDimension: Int

The maximum image dimension to use for contour detection.

var detectDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background.

Deprecated

