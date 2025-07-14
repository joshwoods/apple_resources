

- AVFoundation
- AVAsynchronousCIImageFilteringRequest
-  renderSize 

Instance Property

# renderSize

The width and height, in pixels, of the frame being processed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var renderSize: CGSize { get }
```

## Discussion

You can use this property if you need to work with Core Image filters that apply transforms to the image.

## See Also

### Getting Contextual Information for Filtering

var compositionTime: CMTime

The time in the video composition corresponding to the frame being processed.

