

- AVFoundation
- AVPlayerItemErrorLog
-  extendedLogData() 

Instance Method

# extendedLogData()

Returns a serialized representation of the error log in the Extended Log File Format.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func extendedLogData() -> Data?
```

## Return Value

A serialized representation of the error log in the Extended Log File Format.

## Discussion

This method converts the web server error log into a textual format that conforms to the W3C Extended Log File Format for web server log files. For more information, see http://www.w3.org/pub/WWW/TR/WD-logfile.html.

You can generate a string suitable for console output using:

```
[[NSString alloc] initWithData:[myLog extendedLogData] encoding:[myLog extendedLogDataStringEncoding]]
```

## See Also

### Accessing Error Data

var events: [AVPlayerItemErrorLogEvent]

A chronologically ordered array of player item error log event objects.

var extendedLogDataStringEncoding: UInt

The string encoding of the extended log data.

