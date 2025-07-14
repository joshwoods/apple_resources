

- AVFAudio
- AVAudioSessionDelegate
-  endInterruption() Deprecated

Instance Method

# endInterruption()

Called after your audio session interruption ends.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func endInterruption()
```

Deprecated

No longer supported

## Discussion

The endInterruption(withFlags:) method provides you with more information upon interruption end than this method does. Apple recommends that you use endInterruption(withFlags:) instead of this method.

If you implement the endInterruption(withFlags:) method, that method is called instead of this one when an interruption ends.

To resume using audio after an interruption ends, you must ensure that your audio session is active. AVAudioPlayer and AVAudioRecorder instances reactivate your audio session automatically when an interruption ends. If you are using another audio technology, such as OpenAL, audio units, or audio queues, you must reactivate your audio session yourself before you can again use audio.

You can also use this method to update the user interface and application state, as necessary.

## See Also

### Delegate Methods

func beginInterruption()

Called after your audio session is interrupted.

Deprecated

func endInterruption(withFlags: Int)

Called after your audio session interruption ends, with flags indicating the state of the audio session.

Deprecated

func inputIsAvailableChanged(Bool)

Called after the availability of audio input changes on a device.

Deprecated

