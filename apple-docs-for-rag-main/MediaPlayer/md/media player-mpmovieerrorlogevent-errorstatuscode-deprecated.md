

- Media Player
- MPMovieErrorLogEvent
-  errorStatusCode Deprecated

Instance Property

# errorStatusCode

A unique error code identifier.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var errorStatusCode: Int { get }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

If the error is unknown, the value of this property is negative.

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

var playbackSessionID: String!

A globally unique identifier (GUID) for the playback session.

Deprecated

var errorDomain: String!

The network domain of the error.

Deprecated

var errorComment: String!

A description of the error.

Deprecated

