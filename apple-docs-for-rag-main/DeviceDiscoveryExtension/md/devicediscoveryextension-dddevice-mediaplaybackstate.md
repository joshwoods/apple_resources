

- DeviceDiscoveryExtension
- DDDevice
-  mediaPlaybackState 

Instance Property

# mediaPlaybackState

A playback status for the device’s current media.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
var mediaPlaybackState: DDDevice.MediaPlaybackState { get set }
```

## Discussion

Your app’s extension sets a value for this property to communicate to the system whether the device currently plays media. While the device plays, the system displays an equalizer animation next to the device in the picker UI.

## See Also

### Communicating device content and playback status

var mediaContentTitle: String?

A title for the current media that the device plays.

var mediaContentSubtitle: String?

A subtitle for the current media that the device plays.

enum MediaPlaybackState

States that indicate the status of a device’s media playback.

