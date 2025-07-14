

- AVFoundation
- AVPartialAsyncProperty
-  preferredTransform 

Type Property

# preferredTransform

The asset’s transform preference to apply to its visual content during presentation or processing.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var preferredTransform: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

This value typically, but not always, equals CGAffineTransformIdentity.

## See Also

### Loading Asset Preferences

static var preferredRate: AVAsyncProperty&lt;Root, Float>

The asset’s rate preference for playing its media.

static var preferredVolume: AVAsyncProperty&lt;Root, Float>

The asset’s volume preference for playing its audible media.

static var preferredDisplayCriteria: AVAsyncProperty&lt;Root, AVDisplayCriteria>

The asset’s display mode preference for optimal playback of its content.

class AVDisplayCriteria

An object the system uses to guide the selection of a display mode in tvOS.

