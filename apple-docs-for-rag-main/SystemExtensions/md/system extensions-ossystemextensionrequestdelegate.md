

- System Extensions
-  OSSystemExtensionRequestDelegate 

Protocol

# OSSystemExtensionRequestDelegate

A type that receives updates about the progress of a request.

macOS 10.15+

``` source
protocol OSSystemExtensionRequestDelegate : NSObjectProtocol
```

## Mentioned in 

Installing System Extensions and Drivers

## Topics

### Handling Success and Failure

func request(OSSystemExtensionRequest, didFinishWithResult: OSSystemExtensionRequest.Result)

Tells the delegate that the manager completed the request.

**Required**

enum Result

The result of a completed request, possibly including additional information about the extension’s state.

func request(OSSystemExtensionRequest, didFailWithError: any Error)

Tells the delegate the manager failed to complete the request.

**Required**

### Handling Indeterminate Installs

func requestNeedsUserApproval(OSSystemExtensionRequest)

Tells the delegate that the user must grant approval before the manager can activate the extension.

**Required**

func request(OSSystemExtensionRequest, actionForReplacingExtension: OSSystemExtensionProperties, withExtension: OSSystemExtensionProperties) -> OSSystemExtensionRequest.ReplacementAction

Tells the delegate that the user has a different version of the extension installed on their system.

**Required**

class OSSystemExtensionProperties

Properties that identify a specific version of a system extension.

enum ReplacementAction

Actions for describing how the extension manager should resolve a version conflict.

### Instance Methods

func request(OSSystemExtensionRequest, foundProperties: [OSSystemExtensionProperties])

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Working with a Delegate

var delegate: (any OSSystemExtensionRequestDelegate)?

A delegate to receive updates about the progress of a request.

