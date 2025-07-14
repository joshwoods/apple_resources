

- AVFAudio
- AVAudioSessionDelegate
-  beginInterruption() Deprecated

Instance Method

# beginInterruption()

Called after your audio session is interrupted.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func beginInterruption()
```

Deprecated

No longer supported

## Discussion

By the time this interruption arrives, your audio has already stopped. Your application may be suspended or terminated following an interruption—for example, if a user chooses to take an incoming phone call. Use this method to adjust the user interface, and to save application state, as necessary.

## See Also

### Related Documentation

Audio Session Programming Guide

### Delegate Methods

func endInterruption()

Called after your audio session interruption ends.

Deprecated

func endInterruption(withFlags: Int)

Called after your audio session interruption ends, with flags indicating the state of the audio session.

Deprecated

func inputIsAvailableChanged(Bool)

Called after the availability of audio input changes on a device.

Deprecated

