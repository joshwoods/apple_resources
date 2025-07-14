

- System Extensions
-  OSSystemExtensionManager 

Class

# OSSystemExtensionManager

A type that facilitates activation and deactivation of system extensions.

macOS 10.15+

``` source
class OSSystemExtensionManager
```

## Mentioned in 

Installing System Extensions and Drivers

## Overview

Create an instance of OSSystemExtensionRequest with the class methods on that type, and submit it to the shared instance of the extension manager with submitRequest(_:). Set the delegate on the request to receive the result of the activation or deactivation. The delegate also receives notifications if the user needs to authorize the extension or if a version conflict occurs.

## Topics

### Accessing the Shared Extension Manager

class var shared: OSSystemExtensionManager

The shared instance of the extension manager.

### Submitting Requests

func submitRequest(OSSystemExtensionRequest)

Submits a system extension request to the manager.

class OSSystemExtensionRequest

A request to activate or deactivate a system extension.

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

class OSSystemExtensionRequest

A request to activate or deactivate a system extension.

System Extension Redistributable Entitlement

A Boolean value that indicates whether other development teams may distribute a system extension you create.

