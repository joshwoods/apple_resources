

- AVFoundation
- AVPlayerItemAccessLog
-  events 

Instance Property

# events

A chronologically ordered array of player item access log events.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var events: [AVPlayerItemAccessLogEvent] { get }
```

## Discussion

The array contains AVPlayerItemAccessLogEvent objects that represent the chronological sequence of events contained in the access log.

This property isn’t observable. For more information about key-value observing, see Using Key-Value Observing in Swift.

## See Also

### Accessing Log Data

func extendedLogData() -> Data?

Returns a serialized representation of the access log in the Extended Log File Format.

var extendedLogDataStringEncoding: UInt

The string encoding of the extended log data.

