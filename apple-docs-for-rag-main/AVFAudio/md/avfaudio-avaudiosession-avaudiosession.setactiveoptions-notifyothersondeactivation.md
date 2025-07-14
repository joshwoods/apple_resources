

- AVFAudio
- AVAudioSession
- AVAudioSession.SetActiveOptions
-  notifyOthersOnDeactivation 

Type Property

# notifyOthersOnDeactivation

An option that indicates that the system should notify other apps that you’ve deactivated your app’s audio session.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
static var notifyOthersOnDeactivation: AVAudioSession.SetActiveOptions { get }
```

## Discussion

When passed in the `options` parameter of the setActive(_:options:) instance method, this option indicates that when your audio session deactivates, other audio sessions that had been interrupted by your session can return to their active state.

Only use this option when deactivating your audio session; that is, when you pass a value of false to the setActive(_:options:) instance method.

## Topics

### Options

var AVAudioSessionSetActiveFlags_NotifyOthersOnDeactivation: Int

A flag that indicates that when your audio session deactivates, any audio sessions that your audio session interrupted can reactivate themselves.

Deprecated

