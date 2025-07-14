

- Virtualization
-  VZVirtioSocketListener 

Class

# VZVirtioSocketListener

An object that listens for port-based connection requests from the guest operating system.

macOS 11.0+

``` source
class VZVirtioSocketListener
```

## Overview

Use a VZVirtioSocketListener object to route connection requests to your associated delegate object. The socket listener object handles incoming connection requests from the guest operating system and directs them to the methods of its associated delegate object. You may use the same listener object to monitor connections on multiple ports.

After creating a VZVirtioSocketListener object, assign a custom object to its delegate property. The delegate must implement the VZVirtioSocketListenerDelegate protocol. To connect the listener to a port, call the setSocketListener(_:forPort:) method of your virtual machine’s VZVirtioSocketDevice object.

## Topics

### Responding to new connections

var delegate: (any VZVirtioSocketListenerDelegate)?

The custom object you use to respond to port-based connection attempts.

protocol VZVirtioSocketListenerDelegate

An interface you use to manage connections between the guest operating system and host computer.

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

### Connection management

class VZVirtioSocketConnection

A port-based connection between the guest operating system and the host computer.

