

- System Extensions
-  OSSystemExtensionRequest 

Class

# OSSystemExtensionRequest

A request to activate or deactivate a system extension.

macOS 10.15+

``` source
class OSSystemExtensionRequest
```

## Mentioned in 

Installing System Extensions and Drivers

## Topics

### Creating Requests

class func activationRequest(forExtensionWithIdentifier: String, queue: dispatch_queue_t) -> Self

Creates a request to activate a System Extension.

class func deactivationRequest(forExtensionWithIdentifier: String, queue: dispatch_queue_t) -> Self

Creates a request to deactivate a System Extension.

### Working with a Delegate

var delegate: (any OSSystemExtensionRequestDelegate)?

A delegate to receive updates about the progress of a request.

protocol OSSystemExtensionRequestDelegate

A type that receives updates about the progress of a request.

### Identifying the Target Extension

var identifier: String

The bundle identifier of the target extension.

### Type Methods

class func propertiesRequest(forExtensionWithIdentifier: String, queue: dispatch_queue_t) -> Self

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Extension activation and deactivation

Installing System Extensions and Drivers

Activate system extensions and drivers to make them available to the system, and update or deactivate them as needed.

class OSSystemExtensionManager

A type that facilitates activation and deactivation of system extensions.

System Extension Redistributable Entitlement

A Boolean value that indicates whether other development teams may distribute a system extension you create.

