

- Foundation
- NSMachPort
-  port(withMachPort:options:) 

Type Method

# port(withMachPort:options:)

Creates and returns a port object configured with the specified options and the given Mach port.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func port(
    withMachPort machPort: UInt32,
    options f: NSMachPort.Options = []
) -> Port
```

## Parameters 

`machPort`  

The Mach port for the new port. This parameter should originally be of type mach_port_t.

`f`  

Specifies options for what to do with the underlying port rights when the `NSMachPort` object is invalidated or destroyed. For a list of constants, see `Mach Port Rights`.

## Return Value

An `NSMachPort` object that uses `machPort` to send or receive messages.

## Discussion

Creates the port object if necessary. Depending on the access rights associated with `machPort`, the new port object may be usable only for sending messages.

## See Also

### Creating and Initializing

class func port(withMachPort: UInt32) -> Port

Creates and returns a port object configured with the given Mach port.

init(machPort: UInt32)

Initializes a newly allocated `NSMachPort` object with a given Mach port.

init(machPort: UInt32, options: NSMachPort.Options)

Initializes a newly allocated `NSMachPort` object with a given Mach port and the specified options.

