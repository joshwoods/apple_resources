

- vmnet
-  interface_event_t 

Structure

# interface_event_t

Interface event types.

Mac Catalyst 13.0+macOS 10.10+

``` source
struct interface_event_t
```

## Topics

### Constants

static var VMNET_INTERFACE_PACKETS_AVAILABLE: interface_event_t

### Initializers

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Data Types

enum vmnet_return_t

Values returned by functions in the vmnet Framework.

struct vmpktdesc

Describes a packet.

typealias interface_ref

A virtual network interface.

enum operating_modes_t

The operating modes for an interface.

