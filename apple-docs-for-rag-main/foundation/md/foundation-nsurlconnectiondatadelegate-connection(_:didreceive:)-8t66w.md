

- Foundation
- NSURLConnectionDataDelegate
-  connection(\_:didReceive:) 

Instance Method

# connection(\_:didReceive:)

Sent when the connection has received sufficient data to construct the URL response for its request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func connection(
    _ connection: NSURLConnection,
    didReceive response: URLResponse
)
```

## Parameters 

`connection`  

The connection sending the message.

`response`  

The URL response for the connection’s request. This object is immutable and will not be modified by the URL loading system once it is presented to the delegate.

## Discussion

In rare cases, for example in the case of an HTTP load where the content type of the load data is `multipart/x-mixed-replace`, the delegate will receive more than one `connection:didReceiveResponse:` message. When this happens, discard (or process) all data previously delivered by `connection:didReceiveData:`, and prepare to handle the next part (which could potentially have a different MIME type).

The only case where this message is not sent to the delegate is when the protocol implementation encounters an error before a response could be created.

## See Also

### Related Documentation

URL Loading System

Interact with URLs and communicate with servers using standard Internet protocols.

### Handling Incoming Data

func connection(NSURLConnection, didReceive: Data)

Sent as a connection loads data incrementally.

