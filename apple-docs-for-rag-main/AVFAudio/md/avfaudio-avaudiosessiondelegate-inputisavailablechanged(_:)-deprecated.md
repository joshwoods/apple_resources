

- AVFAudio
- AVAudioSessionDelegate
-  inputIsAvailableChanged(\_:) Deprecated

Instance Method

# inputIsAvailableChanged(\_:)

Called after the availability of audio input changes on a device.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func inputIsAvailableChanged(_ isInputAvailable: Bool)
```

Deprecated

No longer supported

## Parameters 

`isInputAvailable`  

true if audio input is now available, or false if it is not.

## See Also

### Delegate Methods

func beginInterruption()

Called after your audio session is interrupted.

Deprecated

func endInterruption()

Called after your audio session interruption ends.

Deprecated

func endInterruption(withFlags: Int)

Called after your audio session interruption ends, with flags indicating the state of the audio session.

Deprecated

