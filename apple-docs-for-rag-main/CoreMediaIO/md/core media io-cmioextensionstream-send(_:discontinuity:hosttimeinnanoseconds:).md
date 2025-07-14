

- Core Media I/O
- CMIOExtensionStream
-  send(\_:discontinuity:hostTimeInNanoseconds:) 

Instance Method

# send(\_:discontinuity:hostTimeInNanoseconds:)

Sends a media sample to stream client.

Mac Catalyst 15.4+macOS 12.3+

``` source
func send(
    _ sampleBuffer: CMSampleBuffer,
    discontinuity: CMIOExtensionStream.DiscontinuityFlags,
    hostTimeInNanoseconds: UInt64
)
```

## Parameters 

`sampleBuffer`  

A sample buffer that contains the media data to send.

`discontinuity`  

A flag that indicates whether the sample buffer represents a discontinuity boundary.

`hostTimeInNanoseconds`  

The host time in nanoseconds when the stream captured the buffer.

## Discussion

Specify sample buffer timestamps that are relative to the clock timebase specified by the clockType property.

Important

Attempting to send a sample buffer from a sink stream throws an exception.

## See Also

### Processing Data

func consumeSampleBuffer(from: CMIOExtensionClient, completionHandler: (CMSampleBuffer?, UInt64, CMIOExtensionStream.DiscontinuityFlags, Bool, (any Error)?) -> Void)

Consumes a sample buffer from a client.

struct DiscontinuityFlags

Constants that specify the types of discontinuities that can occur in a media stream.

