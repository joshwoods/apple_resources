

- AVFoundation
- AVMutableMovie
-  preferredTransform 

Instance Property

# preferredTransform

The asset’s transform preference to apply to its visual content during presentation or processing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var preferredTransform: CGAffineTransform { get set }
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

