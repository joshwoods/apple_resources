

- Foundation
- StreamDelegate
-  stream(\_:handle:) 

Instance Method

# stream(\_:handle:)

The delegate receives this message when a given event has occurred on a given stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func stream(
    _ aStream: Stream,
    handle eventCode: Stream.Event
)
```

## Parameters 

`aStream`  

The stream on which `streamEvent` occurred.

`eventCode`  

The stream event that occurred.

## Mentioned in 

Uploading streams of data

## Discussion

The delegate receives this message only if `theStream` is scheduled on a run loop. The message is sent on the stream object’s thread. The delegate should examine `streamEvent` to determine the appropriate action it should take.

## See Also

### Related Documentation

Stream Programming Guide

