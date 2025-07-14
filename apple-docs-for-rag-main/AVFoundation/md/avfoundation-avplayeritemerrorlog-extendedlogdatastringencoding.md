

- AVFoundation
- AVPlayerItemErrorLog
-  extendedLogDataStringEncoding 

Instance Property

# extendedLogDataStringEncoding

The string encoding of the extended log data.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var extendedLogDataStringEncoding: UInt { get }
```

## See Also

### Accessing Error Data

var events: [AVPlayerItemErrorLogEvent]

A chronologically ordered array of player item error log event objects.

func extendedLogData() -> Data?

Returns a serialized representation of the error log in the Extended Log File Format.

