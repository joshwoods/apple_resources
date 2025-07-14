

- AVFoundation
- AVPlayerItemAccessLogEvent
-  numberOfMediaRequests 

Instance Property

# numberOfMediaRequests

The number of media read requests from the server to this client.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var numberOfMediaRequests: Int { get }
```

## Discussion

For HTTP live streaming, this property contains the count of media requests downloaded from the server. For progressive-style HTTP media downloads, it contains a count of HTTP `GET` (byte-range) requests for the resource.

The property corresponds to “sc-count”.

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

var numberOfBytesTransferred: Int64

The accumulated number of bytes transferred by the item.

