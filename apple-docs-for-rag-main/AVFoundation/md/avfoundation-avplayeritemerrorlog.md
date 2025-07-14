

- AVFoundation
-  AVPlayerItemErrorLog 

Class

# AVPlayerItemErrorLog

The error log associated with a player item.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVPlayerItemErrorLog
```

## Topics

### Accessing Error Data

var events: [AVPlayerItemErrorLogEvent]

A chronologically ordered array of player item error log event objects.

func extendedLogData() -> Data?

Returns a serialized representation of the error log in the Extended Log File Format.

var extendedLogDataStringEncoding: UInt

The string encoding of the extended log data.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Accessing Logging Information

func accessLog() -> AVPlayerItemAccessLog?

Returns an object that represents a snapshot of the network access log.

class AVPlayerItemAccessLog

An object used to retrieve the access log associated with a player item.

class AVPlayerItemAccessLogEvent

A single entry in a player item’s access log.

func errorLog() -> AVPlayerItemErrorLog?

Returns an object that represents a snapshot of the error log.

class AVPlayerItemErrorLogEvent

A single item in a player item’s error log.

