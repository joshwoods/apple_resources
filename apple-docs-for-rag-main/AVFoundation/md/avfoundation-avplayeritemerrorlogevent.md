

- AVFoundation
-  AVPlayerItemErrorLogEvent 

Class

# AVPlayerItemErrorLogEvent

A single item in a player item’s error log.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVPlayerItemErrorLogEvent
```

## Overview

This object provides properties for accessing the data fields of each log event. Each event is a single entry in an AVPlayerItem object’s error log.

These properties aren’t observable. For more information about key-value observing, see Using Key-Value Observing in Swift.

## Topics

### Getting Information About the Event

var date: Date?

The date and time when the error occurred.

var uri: String?

The URI of the playback item that had an error.

var serverAddress: String?

The IP address of the server that was the source of the error.

var playbackSessionID: String?

A GUID that identifies the playback session that had an error.

var errorStatusCode: Int

A unique error code identifier.

var errorDomain: String

The domain of the error.

var errorComment: String?

A description of the error encountered.

var allHTTPResponseHeaderFields: [String : String]?

The HTTP header fields the server returns.

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

class AVPlayerItemErrorLog

The error log associated with a player item.

