

- AVFoundation
-  AVPlayerItemAccessLog 

Class

# AVPlayerItemAccessLog

An object used to retrieve the access log associated with a player item.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVPlayerItemAccessLog
```

## Overview

An `AVPlayerItemAccessLog` object accumulates key metrics about network playback and presents them as a collection of AVPlayerItemAccessLogEvent instances. Each event instance collates the data that relates to each uninterrupted period of playback.

## Topics

### Accessing Log Data

var events: [AVPlayerItemAccessLogEvent]

A chronologically ordered array of player item access log events.

func extendedLogData() -> Data?

Returns a serialized representation of the access log in the Extended Log File Format.

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

class AVPlayerItemAccessLogEvent

A single entry in a player item’s access log.

func errorLog() -> AVPlayerItemErrorLog?

Returns an object that represents a snapshot of the error log.

class AVPlayerItemErrorLog

The error log associated with a player item.

class AVPlayerItemErrorLogEvent

A single item in a player item’s error log.

