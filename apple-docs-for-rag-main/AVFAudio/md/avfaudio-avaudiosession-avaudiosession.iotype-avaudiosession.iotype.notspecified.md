

- AVFAudio
- AVAudioSession
- AVAudioSession.IOType
-  AVAudioSession.IOType.notSpecified 

Case

# AVAudioSession.IOType.notSpecified

The default audio session I/O type.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
case notSpecified
```

## Discussion

Use this I/O type if your app doesn’t use AVCaptureSession, or doesn’t have any specific requirements for aggregating input and output audio in the same realtime I/O callback. If your app doesn’t use a capture session, it gets aggregated I/O when using the playAndRecord category.

If your app uses a capture session, specifying this value allows the session to start recording without causing glitches in the already running output audio. It also allows the system to use power-saving optimizations.

## See Also

### I/O Types

case aggregated

An I/O type that indicates if audio input and output should be presented in the same realtime I/O callback.

