

- Foundation
- NSMachPort
-  machPort 

Instance Property

# machPort

The Mach port used by the receiver, represented as an integer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var machPort: UInt32 { get }
```

## Discussion

The Mach port used by the receiver. Cast this value to a mach_port_t when using it with Mach system calls.

