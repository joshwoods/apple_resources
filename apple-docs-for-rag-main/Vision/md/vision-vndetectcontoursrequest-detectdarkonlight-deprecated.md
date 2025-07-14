

- Vision
- VNDetectContoursRequest
-  detectDarkOnLight Deprecated

Instance Property

# detectDarkOnLight

A Boolean value that indicates whether the request detects a dark object on a light background.

iOS 14.0–14.0DeprecatediPadOS 14.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 11.0–11.0DeprecatedtvOS 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var detectDarkOnLight: Bool { get set }
```

Deprecated

Use detectsDarkOnLight instead.

## Discussion

The default value is true.

## See Also

### Configuring the Request

var contrastAdjustment: Float

The amount by which to adjust the image contrast.

var contrastPivot: NSNumber?

The pixel value to use as a pivot for the contrast.

var detectsDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background to aid in detection.

var maximumImageDimension: Int

The maximum image dimension to use for contour detection.

