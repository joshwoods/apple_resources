

- Network
-  NWInterface 

Structure

# NWInterface

An interface that a network connection uses to send and receive data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct NWInterface
```

## Topics

### Inspecting Interfaces

var type: NWInterface.InterfaceType

The type of the interface, such as Wi-Fi or loopback.

enum InterfaceType

Types of network interfaces, based on their link layer media types.

var name: String

The name of the interface.

var index: Int

The system interface index associated with the interface.

### Enumerations

enum RadioType

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Paths and Interfaces

struct NWPath

An object that contains information about the properties of the network that a connection uses, or that are available to your app.

class NWPathMonitor

An observer that you use to monitor and react to network changes.

