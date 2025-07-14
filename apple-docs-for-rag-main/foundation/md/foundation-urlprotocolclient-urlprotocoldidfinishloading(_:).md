

- Foundation
- URLProtocolClient
-  urlProtocolDidFinishLoading(\_:) 

Instance Method

# urlProtocolDidFinishLoading(\_:)

Tells the client that the protocol implementation has finished loading.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urlProtocolDidFinishLoading(_ protocol: URLProtocol)
```

**Required**

## Parameters 

`protocol`  

The URL protocol object sending the message.

## See Also

### Indicating loading progress or failure

func urlProtocol(URLProtocol, didFailWithError: any Error)

Tells the client that the load request failed due to an error.

**Required**

func urlProtocol(URLProtocol, didLoad: Data)

Tells the client that the protocol implementation has loaded some data.

**Required**

