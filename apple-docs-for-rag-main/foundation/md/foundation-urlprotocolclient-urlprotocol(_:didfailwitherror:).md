

- Foundation
- URLProtocolClient
-  urlProtocol(\_:didFailWithError:) 

Instance Method

# urlProtocol(\_:didFailWithError:)

Tells the client that the load request failed due to an error.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urlProtocol(
    _ protocol: URLProtocol,
    didFailWithError error: any Error
)
```

**Required**

## Parameters 

`protocol`  

The URL protocol object sending the message.

`error`  

The error that caused the failure of the load request.

## See Also

### Indicating loading progress or failure

func urlProtocol(URLProtocol, didLoad: Data)

Tells the client that the protocol implementation has loaded some data.

**Required**

func urlProtocolDidFinishLoading(URLProtocol)

Tells the client that the protocol implementation has finished loading.

**Required**

