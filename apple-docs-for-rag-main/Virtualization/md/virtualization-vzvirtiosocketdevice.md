

- Virtualization
-  VZVirtioSocketDevice 

Class

# VZVirtioSocketDevice

A device that manages port-based connections between the guest system and the host computer.

macOS 11.0+

``` source
class VZVirtioSocketDevice
```

## Overview

Use a VZVirtioSocketDevice object to configure services and other communication end points in your virtual machine. Host computers make services available using ports, which identify the type of service and the protocol to use when transmitting data. Use this object to specify the ports available to your guest operating system, and to register handlers to manage the communication on those ports.

Don’t create a VZVirtioSocketDevice object directly. Instead, when you request a socket device in your configuration, the virtual machine creates it and stores it in the socketDevices property. For each port you want to make available in your virtual machine, call the setSocketListener(_:forPort:) method and provide an object to manage the port connections.

## Topics

### Configuring Port Listeners

func setSocketListener(VZVirtioSocketListener, forPort: UInt32)

Configures an object to monitor the specified port for new connections.

func removeSocketListener(forPort: UInt32)

Removes the listener object from the specfied port.

### Connecting to Guest System Ports

func connect(toPort: UInt32, completionHandler: (Result&lt;VZVirtioSocketConnection, any Error>) -> Void)

Initiates a connection to the specified port of the guest operating system.

func connect(toPort: UInt32) async throws -> VZVirtioSocketConnection

Initiates a connection to the specified port of the guest operating system.

## Relationships

### Inherits From

- VZSocketDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Devices

class VZSocketDevice

The common behavior of socket devices.

