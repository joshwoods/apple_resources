

- AVFAudio
- AVAudioSessionDelegate
-  endInterruption(withFlags:) Deprecated

Instance Method

# endInterruption(withFlags:)

Called after your audio session interruption ends, with flags indicating the state of the audio session.

Mac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func endInterruption(withFlags flags: Int)
```

## Parameters 

`flags`  

Flags indicating the state of the audio session when this method is called. Flags are described in Interruption Flags.

## Discussion

To resume using audio after an interruption ends, you must ensure that your audio session is active. AVAudioPlayer and AVAudioRecorder instances reactivate your audio session automatically when an interruption ends. If you are using another audio technology, such as OpenAL, audio units, or audio queues, you must reactivate your audio session yourself before you can again use audio.

You can also use this method to update the user interface and application state, as necessary.

If this delegate method receives the AVAudioSessionInterruptionFlags_ShouldResume constant in its `flags` parameter, the audio session is immediately ready to be used.

If you implement this method, it is called instead of the endInterruption() method when an interruption ends.

## See Also

### Delegate Methods

func beginInterruption()

Called after your audio session is interrupted.

Deprecated

func endInterruption()

Called after your audio session interruption ends.

Deprecated

func inputIsAvailableChanged(Bool)

Called after the availability of audio input changes on a device.

Deprecated

