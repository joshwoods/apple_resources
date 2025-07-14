

- AVFAudio
- AVAudioRecorder
-  currentTime 

Instance Property

# currentTime

The time, in seconds, since the beginning of the recording.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
var currentTime: TimeInterval { get }
```

## Discussion

The value of this property is `0` when you call it on a stopped audio recorder.

## See Also

### Accessing recorder timing

var deviceCurrentTime: TimeInterval

The time, in seconds, of the host audio device.

