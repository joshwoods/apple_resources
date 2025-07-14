

- Core Image
- CITextFeature
-  subFeatures 

Instance Property

# subFeatures

An array containing additional features detected within the feature.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var subFeatures: [Any]? { get }
```

## Discussion

A text detector can identify both a major region that is likely to contain text as well as the areas within that region that likely to contain individual text features. Such features might be single characters, groups of closely-packed characters, or entire words.

Core Image populates this array only if you enable the CIDetectorReturnSubFeatures option when retrieving features.

