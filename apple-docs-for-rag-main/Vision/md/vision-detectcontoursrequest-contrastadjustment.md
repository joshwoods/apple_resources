

- Vision
- DetectContoursRequest
-  contrastAdjustment 

Instance Property

# contrastAdjustment

The amount by which to adjust the image contrast.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var contrastAdjustment: Float
```

## Discussion

Contour detection works best with high-contrast images. The default value of this property is `2.0`, which doubles the image contrast to achieve the most accurate results.

This property supports a value range from `0.0` to `3.0`.

## See Also

### Inspecting a request

var contrastPivot: Float?

The pixel value to use as a pivot for the contrast.

var detectsDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background to aid in detection.

var maximumImageDimension: Int

The maximum image dimension to use for contour detection.

