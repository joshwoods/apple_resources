

- AVFoundation
- AVPlayerItemAccessLog
-  extendedLogDataStringEncoding 

Instance Property

# extendedLogDataStringEncoding

The string encoding of the extended log data.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var extendedLogDataStringEncoding: UInt { get }
```

## See Also

### Accessing Log Data

var events: [AVPlayerItemAccessLogEvent]

A chronologically ordered array of player item access log events.

func extendedLogData() -> Data?

Returns a serialized representation of the access log in the Extended Log File Format.

