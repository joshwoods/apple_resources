

- AVFAudio
- AVAudioSession
-  spatialPlaybackCapabilitiesChangedNotification 

Type Property

# spatialPlaybackCapabilitiesChangedNotification

A notification the system posts when its spatial playback capabilities change.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class let spatialPlaybackCapabilitiesChangedNotification: NSNotification.Name
```

## Discussion

The system posts this notification when spatial playback capabilities change due to a change in user preference.

The `userInfo` dictionary of this notification contains the AVAudioSessionSpatialAudioEnabledKey key, which indicates whether spatial audio is in an enabled state.

A route change may result in a change in the ability for the system to play spatial audio, so observe routeChangeNotification and use the isSpatialAudioEnabled property to check if the current route supports spatialized playback.

## Topics

### User Info Keys

let AVAudioSessionSpatialAudioEnabledKey: String

A user info key that you use to retrieve the state of spatial playback.

