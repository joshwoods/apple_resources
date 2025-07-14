

- Vision
- DetectContoursRequest
-  detectsDarkOnLight 

Instance Property

# detectsDarkOnLight

A Boolean value that indicates whether the request detects a dark object on a light background to aid in detection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var detectsDarkOnLight: Bool
```

## Discussion

The default value is `true`.

## See Also

### Inspecting a request

var contrastAdjustment: Float

The amount by which to adjust the image contrast.

var contrastPivot: Float?

The pixel value to use as a pivot for the contrast.

var maximumImageDimension: Int

The maximum image dimension to use for contour detection.

