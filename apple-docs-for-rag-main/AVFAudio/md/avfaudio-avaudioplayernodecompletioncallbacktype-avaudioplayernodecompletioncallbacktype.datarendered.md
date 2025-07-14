

- AVFAudio
- AVAudioPlayerNodeCompletionCallbackType
-  AVAudioPlayerNodeCompletionCallbackType.dataRendered 

Case

# AVAudioPlayerNodeCompletionCallbackType.dataRendered

A completion handler that indicates the player renders the buffer or file data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case dataRendered
```

## Discussion

This case doesn’t account for any signal processing latencies downstream of the player in the engine.

## See Also

### Completion Handler Cases

case dataConsumed

A completion handler that indicates the player consumes the buffer or file data.

case dataPlayedBack

A completion handler that indicates the player finishes the buffer or file data.

