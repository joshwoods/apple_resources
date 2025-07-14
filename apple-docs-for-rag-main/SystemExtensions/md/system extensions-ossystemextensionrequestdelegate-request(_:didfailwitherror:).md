

- System Extensions
- OSSystemExtensionRequestDelegate
-  request(\_:didFailWithError:) 

Instance Method

# request(\_:didFailWithError:)

Tells the delegate the manager failed to complete the request.

macOS 10.15+

``` source
func request(
    _ request: OSSystemExtensionRequest,
    didFailWithError error: any Error
)
```

**Required**

## Parameters 

`request`  

The request that failed.

`error`  

The reason the request failed.

## Mentioned in 

Installing System Extensions and Drivers

## See Also

### Handling Success and Failure

func request(OSSystemExtensionRequest, didFinishWithResult: OSSystemExtensionRequest.Result)

Tells the delegate that the manager completed the request.

**Required**

enum Result

The result of a completed request, possibly including additional information about the extension’s state.

