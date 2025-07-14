

- AVFoundation
- AVComposition
-  preferredMediaSelection 

Instance Property

# preferredMediaSelection

The default media selections for this asset’s media selection groups.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var preferredMediaSelection: AVMediaSelection { get }
```

## Discussion

Provides an instance of AVMediaSelection with the default selections for each of the assets media selection groups.

## See Also

### Inspecting Preferences

var preferredRate: Float

The asset’s rate preference for playing its media.

var preferredVolume: Float

The asset’s volume preference for playing its audible media.

var preferredTransform: CGAffineTransform

The asset’s transform preference to apply to its visual content during presentation or processing.

var preferredDisplayCriteria: AVDisplayCriteria

The asset’s display mode preference for optimal playback of its content.

