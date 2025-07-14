

- GameKit
- GKVoiceChatService
-  remoteParticipantVolume Deprecated

Instance Property

# remoteParticipantVolume

A float that scales the volume of all remote participants.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var remoteParticipantVolume: Float { get set }
```

Deprecated

Use SharePlay instead

## Discussion

The value should be between `0.0` (muted) and `1.0` (full volume). The default is `1.0`.

## See Also

### Adjusting Audio Properties

var isMicrophoneMuted: Bool

A Boolean value that determines whether the user’s microphone is muted.

Deprecated

