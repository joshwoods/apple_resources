

- AVFoundation
- AVCaptureSession
-  usesApplicationAudioSession 

Instance Property

# usesApplicationAudioSession

A Boolean value that indicates whether the capture session uses the app’s shared audio session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var usesApplicationAudioSession: Bool { get set }
```

## Discussion

The default value is true. If you set the value to false, the capture session uses a private AVAudioSession instance for audio recording, which may cause interruptions if your app uses its own audio session for playback.

## See Also

### Sharing the Application’s Audio Session

var automaticallyConfiguresApplicationAudioSession: Bool

A Boolean value that indicates whether the capture session automatically changes settings in the app’s shared audio session.

var configuresApplicationAudioSessionToMixWithOthers: Bool

A Boolean value that Indicates whether the capture session configures the app’s audio session to mix with others.

