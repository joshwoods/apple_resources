

- AVFoundation
- AVCaptureSession
-  configuresApplicationAudioSessionToMixWithOthers 

Instance Property

# configuresApplicationAudioSessionToMixWithOthers

A Boolean value that Indicates whether the capture session configures the app’s audio session to mix with others.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+

``` source
var configuresApplicationAudioSessionToMixWithOthers: Bool { get set }
```

## Discussion

By default, a capture session’s audio session interrupts the audio of other apps. To enable background audio from other apps to continue while capturing video, set this value to true.

Note

This property value has no effect when the value of usesApplicationAudioSession is false. It also has no effect on Live Photo movie complement capture (where music is always mixed).

The default value is false.

## See Also

### Sharing the Application’s Audio Session

var usesApplicationAudioSession: Bool

A Boolean value that indicates whether the capture session uses the app’s shared audio session.

var automaticallyConfiguresApplicationAudioSession: Bool

A Boolean value that indicates whether the capture session automatically changes settings in the app’s shared audio session.

