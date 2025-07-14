

- Foundation
- NSURLConnectionDataDelegate
-  connection(\_:didReceive:) 

Instance Method

# connection(\_:didReceive:)

Sent as a connection loads data incrementally.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func connection(
    _ connection: NSURLConnection,
    didReceive data: Data
)
```

## Parameters 

`connection`  

The connection sending the message.

`data`  

The newly available data. The delegate should concatenate the contents of each `data` object delivered to build up the complete data for a URL load.

## Discussion

This method provides the only way for an asynchronous delegate to retrieve the loaded data. It is the responsibility of the delegate to retain or copy this data as it is delivered.

## See Also

### Handling Incoming Data

func connection(NSURLConnection, didReceive: URLResponse)

Sent when the connection has received sufficient data to construct the URL response for its request.

