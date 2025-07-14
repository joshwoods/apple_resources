

- Media Player
- MPMovieAccessLog
-  extendedLogData Deprecated

Instance Property

# extendedLogData

A textual version of the web server access log for the associated movie player.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var extendedLogData: Data! { get }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

The web server access log in a textual format that conforms to the W3C Extended Log File Format for web server log files. For more information, see http://www.w3.org/pub/WWW/TR/WD-logfile.html.

## See Also

### Movie access log properties

var extendedLogDataStringEncoding: UInt

The string encoding for the extendedLogData property.

Deprecated

var events: [Any]!

The events in the movie access log.

Deprecated

