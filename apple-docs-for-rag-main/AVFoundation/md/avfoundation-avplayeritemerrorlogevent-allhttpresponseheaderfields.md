

- AVFoundation
- AVPlayerItemErrorLogEvent
-  allHTTPResponseHeaderFields 

Instance Property

# allHTTPResponseHeaderFields

The HTTP header fields the server returns.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+tvOS 17.5+visionOS 1.2+watchOS 10.5+

``` source
var allHTTPResponseHeaderFields: [String : String]? { get }
```

## See Also

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

