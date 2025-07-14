

- AVFAudio
- AVAudioSession
- AVAudioSession.IOType
-  AVAudioSession.IOType.aggregated 

Case

# AVAudioSession.IOType.aggregated

An I/O type that indicates if audio input and output should be presented in the same realtime I/O callback.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
case aggregated
```

## Discussion

Use this value if your session uses playAndRecord and requires input and output audio to be presented in the same realtime I/O callback. For example, if your app uses a Remote I/O with both input and output enabled.

An audio session’s preference to use aggregated I/O won’t be honored if it specifies the mixWithOthers option and another app’s audio session was already active with nonmixable, nonaggregated I/O.

## See Also

### I/O Types

case notSpecified

The default audio session I/O type.

