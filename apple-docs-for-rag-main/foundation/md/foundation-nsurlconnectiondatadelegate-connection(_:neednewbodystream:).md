

- Foundation
- NSURLConnectionDataDelegate
-  connection(\_:needNewBodyStream:) 

Instance Method

# connection(\_:needNewBodyStream:)

Called when an `NSURLConnection` needs to retransmit a request that has a body stream to provide a new, unopened stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func connection(
    _ connection: NSURLConnection,
    needNewBodyStream request: URLRequest
) -> InputStream?
```

## Parameters 

`connection`  

The NSURLConnection that is requesting a new body stream.

## Return Value

This delegate method should return a new, unopened stream that provides the body contents for the request.

If this delegate method returns `NULL`, the connection fails.

## Discussion

In macOS, if this method is not implemented, body stream data is spooled to disk in case retransmission is required. This spooling may not be desirable for large data sets.

By implementing this delegate method, the client opts out of automatic spooling, and must provide a new, unopened stream for each retransmission.

## See Also

### Handling Redirects

func connection(NSURLConnection, willSend: URLRequest, redirectResponse: URLResponse?) -> URLRequest?

Sent when the connection determines that it must change URLs in order to continue loading a request.

