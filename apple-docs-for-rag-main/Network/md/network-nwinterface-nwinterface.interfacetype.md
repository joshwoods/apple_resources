

- Network
- NWInterface
-  NWInterface.InterfaceType 

Enumeration

# NWInterface.InterfaceType

Types of network interfaces, based on their link layer media types.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum InterfaceType
```

## Topics

### Interface Types

case wifi

The network interface type used for communication over Wi-Fi networks.

case cellular

The network interface type used for communication over cellular networks.

case wiredEthernet

The network interface type used for communication over wired Ethernet networks.

case loopback

The network interface type used for communication over local loopback networks.

case other

The network interface type used for communication over virtual networks or networks of unknown types.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting Interfaces

var type: NWInterface.InterfaceType

The type of the interface, such as Wi-Fi or loopback.

var name: String

The name of the interface.

var index: Int

The system interface index associated with the interface.

