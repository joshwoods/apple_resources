

- Vision
- DetectContoursRequest
-  maximumImageDimension 

Instance Property

# maximumImageDimension

The maximum image dimension to use for contour detection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var maximumImageDimension: Int
```

## Discussion

Contour detection is computationally intensive. To improve performance, the framework scales the input image down, while maintaining its aspect ratio, such that its maximum dimension is the value of this property. The framework never scales the image up, so specifying the maximum value ensures that the image processes in its original size and not as a downscaled version.

This minimum value supported is `64`. The default value is `512`.

## See Also

### Inspecting a request

var contrastAdjustment: Float

The amount by which to adjust the image contrast.

var contrastPivot: Float?

The pixel value to use as a pivot for the contrast.

var detectsDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background to aid in detection.

