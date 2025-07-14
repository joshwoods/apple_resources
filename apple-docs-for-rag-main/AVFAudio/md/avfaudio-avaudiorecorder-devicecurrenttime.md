

- AVFAudio
- AVAudioRecorder
-  deviceCurrentTime 

Instance Property

# deviceCurrentTime

The time, in seconds, of the host audio device.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
var deviceCurrentTime: TimeInterval { get }
```

## Discussion

Use this property value to schedule audio recording using the record(atTime:) and record(atTime:forDuration:) methods.

## See Also

### Accessing recorder timing

var currentTime: TimeInterval

The time, in seconds, since the beginning of the recording.

