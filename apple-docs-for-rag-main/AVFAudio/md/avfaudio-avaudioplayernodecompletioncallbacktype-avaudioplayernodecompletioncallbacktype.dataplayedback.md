

- AVFAudio
- AVAudioPlayerNodeCompletionCallbackType
-  AVAudioPlayerNodeCompletionCallbackType.dataPlayedBack 

Case

# AVAudioPlayerNodeCompletionCallbackType.dataPlayedBack

A completion handler that indicates the player finishes the buffer or file data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case dataPlayedBack
```

## Discussion

The completion handler is applicable when the engine is rendering to or from an audio device.

It accounts for both signal processing latencies downstream of the player in the engine, and (possibly significant) latency in the audio playback device.

## See Also

### Completion Handler Cases

case dataConsumed

A completion handler that indicates the player consumes the buffer or file data.

case dataRendered

A completion handler that indicates the player renders the buffer or file data.

