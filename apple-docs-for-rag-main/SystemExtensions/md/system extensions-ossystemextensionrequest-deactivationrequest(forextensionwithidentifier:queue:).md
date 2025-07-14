

- System Extensions
- OSSystemExtensionRequest
-  deactivationRequest(forExtensionWithIdentifier:queue:) 

Type Method

# deactivationRequest(forExtensionWithIdentifier:queue:)

Creates a request to deactivate a System Extension.

macOS 10.15+

``` source
class func deactivationRequest(
    forExtensionWithIdentifier identifier: String,
    queue: dispatch_queue_t
) -> Self
```

## Parameters 

`identifier`  

The bundle identifier of the extension to deactivate.

`queue`  

The dispatch queue to use when calling delegate methods.

## Mentioned in 

Installing System Extensions and Drivers

## Discussion

The system discovers existing system extensions in the `Contents/Library/SystemExtensions` directory of the main app bundle.

A deactivation request may require a restart before deactivating the extension. If the request succeeds but requires a restart to complete, the extension may still appear operational until the next restart.

## See Also

### Creating Requests

class func activationRequest(forExtensionWithIdentifier: String, queue: dispatch_queue_t) -> Self

Creates a request to activate a System Extension.

