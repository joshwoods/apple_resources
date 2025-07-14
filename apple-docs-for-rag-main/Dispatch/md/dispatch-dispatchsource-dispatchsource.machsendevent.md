

- Dispatch
- DispatchSource
-  DispatchSource.MachSendEvent 

Structure

# DispatchSource.MachSendEvent

Mach-related events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MachSendEvent
```

## Topics

### Mach Event Flags

static let dead: DispatchSource.MachSendEvent

The receive right corresponding to the given send right was destroyed.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating a Mach Port Source

class func makeMachReceiveSource(port: mach_port_t, queue: DispatchQueue?) -> any DispatchSourceMachReceive

Creates a new dispatch source object for monitoring a Mach port for pending messages.

class func makeMachSendSource(port: mach_port_t, eventMask: DispatchSource.MachSendEvent, queue: DispatchQueue?) -> any DispatchSourceMachSend

A dispatch source that monitors a Mach port for dead name notifications.

protocol DispatchSourceMachReceive

A dispatch source that monitors a Mach port for pending messages.

protocol DispatchSourceMachSend

A dispatch source that monitors a Mach port for dead name notifications, indicating that a send right no longer has a corresponding receive right.

