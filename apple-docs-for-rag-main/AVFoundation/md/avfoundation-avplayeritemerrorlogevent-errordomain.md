

- AVFoundation
- AVPlayerItemErrorLogEvent
-  errorDomain 

Instance Property

# errorDomain

The domain of the error.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var errorDomain: String { get }
```

## Discussion

The property corresponds to “domain”.

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

var errorComment: String?

A description of the error encountered.

var allHTTPResponseHeaderFields: [String : String]?

The HTTP header fields the server returns.

