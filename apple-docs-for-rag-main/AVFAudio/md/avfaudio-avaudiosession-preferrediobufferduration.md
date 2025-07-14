

- AVFAudio
- AVAudioSession
-  preferredIOBufferDuration 

Instance Property

# preferredIOBufferDuration

The preferred I/O buffer duration, in seconds.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var preferredIOBufferDuration: TimeInterval { get }
```

## Discussion

The value of this property indicates the buffer duration selected using the setPreferredIOBufferDuration(_:) method.

To determine the actual buffer duration, query the ioBufferDuration property.

## See Also

### Configuring I/O buffer duration

var ioBufferDuration: TimeInterval

The current I/O buffer duration, in seconds.

func setPreferredIOBufferDuration(TimeInterval) throws

Sets the preferred audio I/O buffer duration.

