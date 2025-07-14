

- Vision
- VNDetectHumanHandPoseRequest
-  maximumHandCount 

Instance Property

# maximumHandCount

The maximum number of hands to detect in an image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var maximumHandCount: Int { get set }
```

## Discussion

The request orders detected hands by relative size, with only the largest ones having key points determined.

The default value is 2.

