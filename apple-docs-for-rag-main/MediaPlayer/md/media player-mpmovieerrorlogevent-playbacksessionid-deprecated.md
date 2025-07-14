

- Media Player
- MPMovieErrorLogEvent
-  playbackSessionID Deprecated

Instance Property

# playbackSessionID

A globally unique identifier (GUID) for the playback session.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var playbackSessionID: String! { get }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

HTTP requests use the GUID.

## See Also

### Movie error log event properties

var date: Date!

The date and time when the error occurred.

Deprecated

var uri: String!

The URI of the item playing when the error occurred.

Deprecated

var serverAddress: String!

The IP address of the web server that was the source of the error.

Deprecated

var errorStatusCode: Int

A unique error code identifier.

Deprecated

var errorDomain: String!

The network domain of the error.

Deprecated

var errorComment: String!

A description of the error.

Deprecated

