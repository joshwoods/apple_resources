

- System Extensions
- OSSystemExtensionRequestDelegate
-  request(\_:didFinishWithResult:) 

Instance Method

# request(\_:didFinishWithResult:)

Tells the delegate that the manager completed the request.

macOS 10.15+

``` source
func request(
    _ request: OSSystemExtensionRequest,
    didFinishWithResult result: OSSystemExtensionRequest.Result
)
```

**Required**

## Parameters 

`request`  

The request that completed.

`result`  

Additional information about the completion state.

## Discussion

If the request completes with the OSSystemExtensionRequest.Result.willCompleteAfterReboot result, then the extension isn’t active until after the next restart. After restarting, the most recently-processed request determines the extension’s state. Consider the following scenarios:

- Activate extension and restart: the extension is active upon restarting.

- Activate extension, deactivate extension, and restart: the extension is inactive upon restarting.

## See Also

### Handling Success and Failure

enum Result

The result of a completed request, possibly including additional information about the extension’s state.

func request(OSSystemExtensionRequest, didFailWithError: any Error)

Tells the delegate the manager failed to complete the request.

**Required**

