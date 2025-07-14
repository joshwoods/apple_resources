

- AVKit
- AVPlayerViewController
-  speeds 

Instance Property

# speeds

A list of user-selectable playback speeds to show in the playback speed control.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var speeds: [AVPlaybackSpeed] { get set }
```

## Discussion

By default, this property value equals systemDefaultSpeeds. Setting this property to an empty array hides the playback speed selection user interface.

To set the playback speed programmatically, call the selectSpeed(_:) method, or set the value of the defaultRate property on the view controller’s associated player object.

## See Also

### Configuring Playback Speed

var selectedSpeed: AVPlaybackSpeed?

The currently selected playback speed.

func selectSpeed(AVPlaybackSpeed)

Selects a specified playback speed.

class AVPlaybackSpeed

An object that represents a user-selectable playback speed in a playback user interface.

