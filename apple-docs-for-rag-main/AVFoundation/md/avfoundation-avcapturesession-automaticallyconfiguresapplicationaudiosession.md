

- AVFoundation
- AVCaptureSession
-  automaticallyConfiguresApplicationAudioSession 

Instance Property

# automaticallyConfiguresApplicationAudioSession

A Boolean value that indicates whether the capture session automatically changes settings in the app’s shared audio session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var automaticallyConfiguresApplicationAudioSession: Bool { get set }
```

## Discussion

This property only takes effect if the value of the usesApplicationAudioSession property is true.

The value of this property defaults to true, causing the capture session to automatically configure the app’s shared AVAudioSession instance for optimal recording. For example, if the capture session uses a device’s rear-facing camera, the system sets the audio session’s microphone and polar pattern for optimal recording of sound from that direction. The audio session’s original state isn’t restored after capture finishes.

If you set value to false, your app is responsible for selecting appropriate audio session settings. Recording may fail if the audio session’s settings are incompatible with the capture session.

## See Also

### Sharing the Application’s Audio Session

var usesApplicationAudioSession: Bool

A Boolean value that indicates whether the capture session uses the app’s shared audio session.

var configuresApplicationAudioSessionToMixWithOthers: Bool

A Boolean value that Indicates whether the capture session configures the app’s audio session to mix with others.

