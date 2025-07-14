

- AVFAudio
-  AVAudioSessionSetActiveFlags_NotifyOthersOnDeactivation Deprecated

Global Variable

# AVAudioSessionSetActiveFlags_NotifyOthersOnDeactivation

A flag that indicates that when your audio session deactivates, any audio sessions that your audio session interrupted can reactivate themselves.

visionOS 1.0–1.0Deprecated

``` source
var AVAudioSessionSetActiveFlags_NotifyOthersOnDeactivation: Int { get }
```

Deprecated

Use the constants in AVAudioSession.SetActiveOptions instead.

## Discussion

This flag works when passed in the `flags` parameter of the setActive(_:withFlags:) instance method. You use this flag only when deactivating your audio session.

