

- vmnet
-  vmnet_return_t 

Enumeration

# vmnet_return_t

Values returned by functions in the vmnet Framework.

Mac Catalyst 13.0+macOS 10.10+

``` source
enum vmnet_return_t
```

## Topics

### Constants

case VMNET_SUCCESS

case VMNET_FAILURE

case VMNET_MEM_FAILURE

case VMNET_INVALID_ARGUMENT

case VMNET_SETUP_INCOMPLETE

case VMNET_INVALID_ACCESS

case VMNET_PACKET_TOO_BIG

case VMNET_BUFFER_EXHAUSTED

case VMNET_TOO_MANY_PACKETS

### Enumeration Cases

case VMNET_NOT_AUTHORIZED

case VMNET_SHARING_SERVICE_BUSY

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data Types

struct vmpktdesc

Describes a packet.

typealias interface_ref

A virtual network interface.

struct interface_event_t

Interface event types.

enum operating_modes_t

The operating modes for an interface.

