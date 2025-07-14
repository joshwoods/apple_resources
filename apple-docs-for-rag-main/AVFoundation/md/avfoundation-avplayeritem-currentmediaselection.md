

- AVFoundation
- AVPlayerItem
-  currentMediaSelection 

Instance Property

# currentMediaSelection

The current media selections for each of the receiver’s media selection groups.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@MainActor
var currentMediaSelection: AVMediaSelection { get }
```

## See Also

### Selecting Media Options

func select(AVMediaSelectionOption?, in: AVMediaSelectionGroup)

Selects a media option in a given media selection group and deselects all other options in that group.

func selectMediaOptionAutomatically(in: AVMediaSelectionGroup)

Selects the media option in the specified media selection group that best matches the receiver’s automatic selection criteria.

