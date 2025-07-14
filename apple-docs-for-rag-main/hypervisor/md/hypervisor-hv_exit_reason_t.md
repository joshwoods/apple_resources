

- Hypervisor
-  hv_exit_reason_t 

Structure

# hv_exit_reason_t

The type that describes the event that triggered a guest exit to the host.

macOS

``` source
struct hv_exit_reason_t
```

## Topics

### Instance Properties

var rawValue: UInt32

The unsigned 32-bit integer that represents virual macine exit reasons.

### Initializers

init(UInt32)

Creates a new exit reason instance with the value you provide.

init(rawValue: UInt32)

Creates a new exit reason instance with the value you provide.

### Exit Reasons

var HV_EXIT_REASON_CANCELED: hv_exit_reason_t

The value that identifies exits requested by exit handler on the host.

var HV_EXIT_REASON_EXCEPTION: hv_exit_reason_t

The value that identifies traps caused by the guest operations.

var HV_EXIT_REASON_VTIMER_ACTIVATED: hv_exit_reason_t

The value that identifies when the virtual timer enters the pending state.

var HV_EXIT_REASON_UNKNOWN: hv_exit_reason_t

The value that identifies unexpected exits.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Exit reasons

typealias hv_exception_syndrome_t

Type of a vCPU exception syndrome.

typealias hv_exception_address_t

Type of a vCPU exception virtual address.

