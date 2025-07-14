

- Core Image
- CIDetector
- Detector Configuration Keys
-  CIDetectorMinFeatureSize 

Global Variable

# CIDetectorMinFeatureSize

A key used to specify the minimum size that the detector will recognize as a feature.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
let CIDetectorMinFeatureSize: String
```

## Discussion

The value for this key is an `NSNumber` object ranging from 0.0 through 1.0 that represents a fraction of the minor dimension of the image.

