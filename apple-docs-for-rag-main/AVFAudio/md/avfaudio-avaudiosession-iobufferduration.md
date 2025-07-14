

- AVFAudio
- AVAudioSession
-  ioBufferDuration 

Instance Property

# ioBufferDuration

The current I/O buffer duration, in seconds.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var ioBufferDuration: TimeInterval { get }
```

## See Also

### Configuring I/O buffer duration

var preferredIOBufferDuration: TimeInterval

The preferred I/O buffer duration, in seconds.

func setPreferredIOBufferDuration(TimeInterval) throws

Sets the preferred audio I/O buffer duration.

