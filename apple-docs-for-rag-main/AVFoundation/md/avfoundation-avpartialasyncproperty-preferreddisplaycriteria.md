

- AVFoundation
- AVPartialAsyncProperty
-  preferredDisplayCriteria 

Type Property

# preferredDisplayCriteria

The asset’s display mode preference for optimal playback of its content.

tvOS 15.0+visionOS 1.0+

``` source
static var preferredDisplayCriteria: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Asset Preferences

static var preferredRate: AVAsyncProperty&lt;Root, Float>

The asset’s rate preference for playing its media.

static var preferredVolume: AVAsyncProperty&lt;Root, Float>

The asset’s volume preference for playing its audible media.

static var preferredTransform: AVAsyncProperty&lt;Root, CGAffineTransform>

The asset’s transform preference to apply to its visual content during presentation or processing.

class AVDisplayCriteria

An object the system uses to guide the selection of a display mode in tvOS.

