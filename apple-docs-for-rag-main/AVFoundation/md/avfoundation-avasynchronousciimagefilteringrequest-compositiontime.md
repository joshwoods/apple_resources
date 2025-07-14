

- AVFoundation
- AVAsynchronousCIImageFilteringRequest
-  compositionTime 

Instance Property

# compositionTime

The time in the video composition corresponding to the frame being processed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var compositionTime: CMTime { get }
```

## Discussion

You can use this property to vary the parameters of a filter over time.

## See Also

### Getting Contextual Information for Filtering

var renderSize: CGSize

The width and height, in pixels, of the frame being processed.

