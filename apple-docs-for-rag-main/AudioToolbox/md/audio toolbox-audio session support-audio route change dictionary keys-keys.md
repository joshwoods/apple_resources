

- Audio Toolbox
- Audio Session Support
-  Audio Route Change Dictionary Keys 

API Collection

# Audio Route Change Dictionary Keys

Keys for obtaining information about an audio hardware route change.

## Topics

### Constants

let kAudioSession_RouteChangeKey_Reason: CFString!

The reason for the audio route change.

Deprecated

let kAudioSession_AudioRouteChangeKey_PreviousRouteDescription: CFString!

Describes the previous audio route.

Deprecated

let kAudioSession_AudioRouteChangeKey_CurrentRouteDescription: CFString!

Describes the current audio route.

Deprecated

## See Also

### Audio Routes

Audio Route Change Reasons

Identifiers for the various reasons that an audio route can change while your app is running.

Audio Route Description Dictionary Keys

Keys for the kAudioSessionProperty_AudioRouteDescription dictionary.

Audio Route Type Key

The one key for an audio route input or output dictionary.

Audio Input Routes

Strings that identify the various audio input sources for a device.

Audio Output Routes

The various audio output destinations available for an iOS device.

Alternative Audio Route Change Reason Dictionary Key

An alternate key for obtaining information about the reason for an audio route change.

