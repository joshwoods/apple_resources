

- AVFoundation
- AVPartialAsyncProperty
-  preferredVolume 

Type Property

# preferredVolume

The asset’s volume preference for playing its audible media.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var preferredVolume: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

The preferred volume for an audio track is typically, but not always, `1.0`. For nonaudible tracks, the value is `0.0`.

## See Also

### Loading Asset Preferences

static var preferredRate: AVAsyncProperty&lt;Root, Float>

The asset’s rate preference for playing its media.

static var preferredTransform: AVAsyncProperty&lt;Root, CGAffineTransform>

The asset’s transform preference to apply to its visual content during presentation or processing.

static var preferredDisplayCriteria: AVAsyncProperty&lt;Root, AVDisplayCriteria>

The asset’s display mode preference for optimal playback of its content.

class AVDisplayCriteria

An object the system uses to guide the selection of a display mode in tvOS.

