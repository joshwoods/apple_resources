

- Dispatch
-  DispatchSourceMachReceive 

Protocol

# DispatchSourceMachReceive

A dispatch source that monitors a Mach port for pending messages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol DispatchSourceMachReceive : DispatchSourceProtocol, Sendable
```

## Overview

You do not adopt this protocol in your objects. Instead, use the makeMachReceiveSource(port:queue:) method to create an object that adopts this protocol.

## Topics

### Getting the Mach Port Handle

var handle: mach_port_t

## Relationships

### Inherits From

- DispatchSourceProtocol
- NSObjectProtocol
- Sendable

### Conforming Types

- DispatchSource

## See Also

### Creating a Mach Port Source

class func makeMachReceiveSource(port: mach_port_t, queue: DispatchQueue?) -> any DispatchSourceMachReceive

Creates a new dispatch source object for monitoring a Mach port for pending messages.

class func makeMachSendSource(port: mach_port_t, eventMask: DispatchSource.MachSendEvent, queue: DispatchQueue?) -> any DispatchSourceMachSend

A dispatch source that monitors a Mach port for dead name notifications.

protocol DispatchSourceMachSend

A dispatch source that monitors a Mach port for dead name notifications, indicating that a send right no longer has a corresponding receive right.

struct MachSendEvent

Mach-related events.

