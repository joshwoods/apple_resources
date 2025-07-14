

- AVFoundation
- AVPlayerItem
-  errorLog() 

Instance Method

# errorLog()

Returns an object that represents a snapshot of the error log.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func errorLog() -> AVPlayerItemErrorLog?
```

## Return Value

An object that represents a snapshot of the error log. The returned value can be `nil`.

## Discussion

If the method returns `nil`, there is no logging information currently available for the player item.

## See Also

### Accessing Logging Information

func accessLog() -> AVPlayerItemAccessLog?

Returns an object that represents a snapshot of the network access log.

class AVPlayerItemAccessLog

An object used to retrieve the access log associated with a player item.

class AVPlayerItemAccessLogEvent

A single entry in a player item’s access log.

class AVPlayerItemErrorLog

The error log associated with a player item.

class AVPlayerItemErrorLogEvent

A single item in a player item’s error log.

