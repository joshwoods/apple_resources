

- Core Image
- CIDetector
- Feature Detection Keys
-  CIDetectorReturnSubFeatures 

Global Variable

# CIDetectorReturnSubFeatures

An option specifying whether to return feature information for components of detected features.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
let CIDetectorReturnSubFeatures: String
```

## Discussion

The value of this key is an `NSNumber` object with a Boolean value. Use this option with the CIDetectorTypeText detector type to choose whether to detect only regions likely to contain text (`false`, the default) or to also identify sub-regions likely to contain individual characters of text (`true`).

