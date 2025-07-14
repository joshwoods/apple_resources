

- AVFoundation
- AVLayerVideoGravity
-  resizeAspectFill 

Type Property

# resizeAspectFill

The video preserves its aspect ratio and fills the layer’s bounds.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
static let resizeAspectFill: AVLayerVideoGravity
```

## Discussion

This gravity value may crop the video image along its horizontal or vertical dimension.

## See Also

### Video Gravities

static let resize: AVLayerVideoGravity

The video stretches to fill the layer’s bounds.

static let resizeAspect: AVLayerVideoGravity

The video preserves its aspect ratio and fits it within the layer’s bounds.

