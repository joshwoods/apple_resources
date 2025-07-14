

- Vision
- VNDetectContoursRequest
-  contrastAdjustment 

Instance Property

# contrastAdjustment

The amount by which to adjust the image contrast.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var contrastAdjustment: Float { get set }
```

## Discussion

Contour detection works best with high-contrast images. The default value of this property is `2.0`, which doubles the image contrast to achieve the most accurate results.

This property supports a value range from `0.0` to `3.0`.

## See Also

### Configuring the Request

var contrastPivot: NSNumber?

The pixel value to use as a pivot for the contrast.

var detectsDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background to aid in detection.

var maximumImageDimension: Int

The maximum image dimension to use for contour detection.

var detectDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background.

Deprecated

