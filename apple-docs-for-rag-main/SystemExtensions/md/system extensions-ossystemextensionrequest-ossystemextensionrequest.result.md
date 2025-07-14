

- System Extensions
- OSSystemExtensionRequest
-  OSSystemExtensionRequest.Result 

Enumeration

# OSSystemExtensionRequest.Result

The result of a completed request, possibly including additional information about the extension’s state.

macOS 10.15+

``` source
enum Result
```

## Topics

### Results

case completed

The request completed successfully.

case willCompleteAfterReboot

The request requires a restart to complete successfully.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling Success and Failure

func request(OSSystemExtensionRequest, didFinishWithResult: OSSystemExtensionRequest.Result)

Tells the delegate that the manager completed the request.

**Required**

func request(OSSystemExtensionRequest, didFailWithError: any Error)

Tells the delegate the manager failed to complete the request.

**Required**

