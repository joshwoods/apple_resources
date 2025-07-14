

- AVFoundation
- AVPlayerItemErrorLogEvent
-  date 

Instance Property

# date

The date and time when the error occurred.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var date: Date? { get }
```

## Discussion

The property corresponds to “date”.

The value of this property may be `nil` if the date is unknown.

## See Also

### Getting Information About the Event

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

