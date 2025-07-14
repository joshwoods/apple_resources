

- DeviceDiscoveryExtension
- DDDevice
-  mediaContentSubtitle 

Instance Property

# mediaContentSubtitle

A subtitle for the current media that the device plays.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
var mediaContentSubtitle: String? { get set }
```

## Discussion

Your app’s extension sets a value for this property to communicate to the system the particular media that the device currently plays. The system displays the information to the user in a Now Playing view in the picker UI.

Set this property to `nil` when mediaPlaybackState is DDDevice.MediaPlaybackState.noContent.

## See Also

### Communicating device content and playback status

var mediaContentTitle: String?

A title for the current media that the device plays.

var mediaPlaybackState: DDDevice.MediaPlaybackState

A playback status for the device’s current media.

enum MediaPlaybackState

States that indicate the status of a device’s media playback.

