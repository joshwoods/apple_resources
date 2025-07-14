

- AVFoundation
- AVPlayerItemAccessLogEvent
-  numberOfBytesTransferred 

Instance Property

# numberOfBytesTransferred

The accumulated number of bytes transferred by the item.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var numberOfBytesTransferred: Int64 { get }
```

## Discussion

The property corresponds to “bytes”.

The value of this property is negative if unknown.

This property is not compatible with key-value observing.

## See Also

### Getting Server-Related Log Events

var uri: String?

The URI of the playback item.

var serverAddress: String?

The IP address of the server that was the source of the last delivered media segment.

var numberOfServerAddressChanges: Int

A count of changes to the server address over the last uninterrupted period of playback.

var mediaRequestsWWAN: Int

The number of network read requests over a WWAN.

var transferDuration: TimeInterval

The accumulated duration, in seconds, of active network transfer of bytes.

var numberOfMediaRequests: Int

The number of media read requests from the server to this client.

