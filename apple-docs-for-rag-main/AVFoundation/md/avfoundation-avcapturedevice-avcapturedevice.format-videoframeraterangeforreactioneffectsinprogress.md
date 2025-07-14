

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoFrameRateRangeForReactionEffectsInProgress 

Instance Property

# videoFrameRateRangeForReactionEffectsInProgress

Indicates the minimum and maximum frame rates available when a reaction effect runs.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var videoFrameRateRangeForReactionEffectsInProgress: AVFrameRateRange? { get }
```

## Discussion

Unlike other video effects, enabling reaction effects doesn’t limit the stream’s frame rate because most of the time the system isn’t rendering the effect. The frame rate only ramps down when the system renders a reaction on the stream.

## See Also

### Determining Reaction Effects Support

var reactionEffectsSupported: Bool

A Boolean value that indicates whether the device supports reaction effects.

