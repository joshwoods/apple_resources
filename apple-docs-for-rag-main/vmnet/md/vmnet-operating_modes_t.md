

- vmnet
-  operating_modes_t 

Enumeration

# operating_modes_t

The operating modes for an interface.

Mac Catalyst 13.0+macOS 10.10+

``` source
enum operating_modes_t
```

## Topics

### Constants

case VMNET_HOST_MODE

case VMNET_SHARED_MODE

### Enumeration cases

case VMNET_BRIDGED_MODE

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

enum vmnet_return_t

Values returned by functions in the vmnet Framework.

struct vmpktdesc

Describes a packet.

typealias interface_ref

A virtual network interface.

struct interface_event_t

Interface event types.

