

- Foundation
- URLProtocolClient
-  urlProtocol(\_:didLoad:) 

Instance Method

# urlProtocol(\_:didLoad:)

Tells the client that the protocol implementation has loaded some data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urlProtocol(
    _ protocol: URLProtocol,
    didLoad data: Data
)
```

**Required**

## Parameters 

`protocol`  

The URL protocol object sending the message.

`data`  

The data being made available.

## Discussion

The data object must contain only new data loaded since the previous invocation of this method.

## See Also

### Indicating loading progress or failure

func urlProtocol(URLProtocol, didFailWithError: any Error)

Tells the client that the load request failed due to an error.

**Required**

func urlProtocolDidFinishLoading(URLProtocol)

Tells the client that the protocol implementation has finished loading.

**Required**

