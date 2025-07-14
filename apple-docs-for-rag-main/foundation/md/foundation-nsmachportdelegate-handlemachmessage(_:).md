

- Foundation
- NSMachPortDelegate
-  handleMachMessage(\_:) 

Instance Method

# handleMachMessage(\_:)

Process an incoming Mach message.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func handleMachMessage(_ msg: UnsafeMutableRawPointer)
```

## Parameters 

`msg`  

A pointer to a Mach message, cast as a pointer to void.

## Discussion

The delegate should interpret this data as a pointer to a Mach message beginning with a msg_header_t structure and should handle the message appropriately.

The delegate should implement either `handleMachMessage:` or the PortDelegate protocol method handlePortMessage:.

## See Also

### Related Documentation

Distributed Objects Programming Topics

