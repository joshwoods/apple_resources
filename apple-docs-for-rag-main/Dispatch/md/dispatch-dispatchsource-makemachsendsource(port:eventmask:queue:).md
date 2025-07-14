

- Dispatch
- DispatchSource
-  makeMachSendSource(port:eventMask:queue:) 

Type Method

# makeMachSendSource(port:eventMask:queue:)

A dispatch source that monitors a Mach port for dead name notifications.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func makeMachSendSource(
    port: mach_port_t,
    eventMask: DispatchSource.MachSendEvent,
    queue: DispatchQueue? = nil
) -> any DispatchSourceMachSend
```

## Parameters 

`port`  

A Mach port with a send or send-once right.

`eventMask`  

The events you want to monitor. For a list of possible values, see DispatchSource.MachSendEvent.

`queue`  

The dispatch queue to use when executing the installed handlers.

## Return Value

A dispatch source object that conforms to the DispatchSourceMachSend protocol.

## Discussion

After creating the dispatch source, use the methods of the DispatchSourceProtocol protocol to install the event handlers you need. The returned dispatch source is in the inactive state initially. When you are ready to begin processing events, call its activate() method.

## See Also

### Creating a Mach Port Source

class func makeMachReceiveSource(port: mach_port_t, queue: DispatchQueue?) -> any DispatchSourceMachReceive

Creates a new dispatch source object for monitoring a Mach port for pending messages.

protocol DispatchSourceMachReceive

A dispatch source that monitors a Mach port for pending messages.

protocol DispatchSourceMachSend

A dispatch source that monitors a Mach port for dead name notifications, indicating that a send right no longer has a corresponding receive right.

struct MachSendEvent

Mach-related events.

