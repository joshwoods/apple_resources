

- Network
-  nw_interface_t 

Type Alias

# nw_interface_t

An interface that a network connection uses to send and receive data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_interface_t = any OS_nw_interface
```

## Topics

### Network Interface Types

struct nw_interface_type_t

Types of network interfaces, based on their link layer media types.

### Inspecting Interfaces

func nw_interface_get_type(nw_interface_t) -> nw_interface_type_t

Accesses the type of the interface, such as Wi-Fi or Loopback.

func nw_interface_get_name(nw_interface_t) -> UnsafePointer&lt;CChar>

Accesses the name of the interface.

func nw_interface_get_index(nw_interface_t) -> UInt32

Accesses the system interface index associated with the interface.

