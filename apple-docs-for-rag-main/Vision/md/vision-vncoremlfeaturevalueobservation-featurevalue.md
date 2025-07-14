

- Vision
- VNCoreMLFeatureValueObservation
-  featureValue 

Instance Property

# featureValue

The feature result of a VNCoreMLRequest that outputs neither a classification nor an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@NSCopying
var featureValue: MLFeatureValue { get }
```

## Discussion

Refer to Core ML documentation and the model itself to learn about proper handling of the content.

## See Also

### Obtaining Feature Values

var featureName: String

The name used in the model description of the CoreML model that produced this observation.

