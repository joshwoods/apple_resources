

- Foundation
-  NSURLConnectionDataDelegate 

Protocol

# NSURLConnectionDataDelegate

A protocol that most delegates of a URL connection implement to receive data associated with the connection.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSURLConnectionDataDelegate : NSURLConnectionDelegate
```

## Overview

The `NSURLConnectionDataDelegate` protocol describes methods that should be implemented by the delegate for an instance of the NSURLConnection class. Many methods in this protocol existed as part of an informal protocol in previous versions of macOS and iOS.

In addition to the methods described in this protocol, an `NSURLConnection` delegate should also implement the methods described in the NSURLConnectionDelegate protocol.

Note

If you are using `NSURLConnection` as part of Newsstand Kit on iOS, you should also implement the methods in the NSURLConnectionDownloadDelegate protocol.

## Topics

### Handling Incoming Data

func connection(NSURLConnection, didReceive: URLResponse)

Sent when the connection has received sufficient data to construct the URL response for its request.

func connection(NSURLConnection, didReceive: Data)

Sent as a connection loads data incrementally.

### Receiving Connection Progress

func connection(NSURLConnection, didSendBodyData: Int, totalBytesWritten: Int, totalBytesExpectedToWrite: Int)

Sent as the body (message data) of a request is transmitted (such as in an HTTP POST request).

func connectionDidFinishLoading(NSURLConnection)

Sent when a connection has finished loading successfully.

### Handling Redirects

func connection(NSURLConnection, willSend: URLRequest, redirectResponse: URLResponse?) -> URLRequest?

Sent when the connection determines that it must change URLs in order to continue loading a request.

func connection(NSURLConnection, needNewBodyStream: URLRequest) -> InputStream?

Called when an `NSURLConnection` needs to retransmit a request that has a body stream to provide a new, unopened stream.

### Overriding Caching Behavior

func connection(NSURLConnection, willCacheResponse: CachedURLResponse) -> CachedURLResponse?

Sent before the connection stores a cached response in the cache, to give the delegate an opportunity to alter it.

## Relationships

### Inherits From

- NSObjectProtocol
- NSURLConnectionDelegate

## See Also

### URL Connection

class NSURLConnection

An object that enables you to start and stop URL requests.

protocol NSURLConnectionDelegate

A protocol that delegates of a URL connection implement to receive status about and provide feedback to the connection object.

protocol NSURLConnectionDownloadDelegate

A protocol that delegates of a URL connection created with Newsstand Kit implement to receive data associated with a download.

