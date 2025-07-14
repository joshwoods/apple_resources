

- AVFoundation
- AVComposition
-  preferredTransform 

Instance Property

# preferredTransform

The asset’s transform preference to apply to its visual content during presentation or processing.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var preferredTransform: CGAffineTransform { get }
```

## Discussion

The value is typically, but not always, the identity transform.

## See Also

### Inspecting Preferences

var preferredRate: Float

The asset’s rate preference for playing its media.

var preferredVolume: Float

The asset’s volume preference for playing its audible media.

var preferredMediaSelection: AVMediaSelection

The default media selections for this asset’s media selection groups.

var preferredDisplayCriteria: AVDisplayCriteria

The asset’s display mode preference for optimal playback of its content.

