

- Foundation
- NSURLConnectionDataDelegate
-  connectionDidFinishLoading(\_:) 

Instance Method

# connectionDidFinishLoading(\_:)

Sent when a connection has finished loading successfully.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func connectionDidFinishLoading(_ connection: NSURLConnection)
```

## Parameters 

`connection`  

The connection sending the message.

## Discussion

The delegate will receive no further messages for `connection`.

## See Also

### Receiving Connection Progress

func connection(NSURLConnection, didSendBodyData: Int, totalBytesWritten: Int, totalBytesExpectedToWrite: Int)

Sent as the body (message data) of a request is transmitted (such as in an HTTP POST request).

