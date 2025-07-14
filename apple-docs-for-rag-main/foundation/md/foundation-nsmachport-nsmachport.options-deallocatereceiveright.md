

- Foundation
- NSMachPort
- NSMachPort.Options
-  deallocateReceiveRight 

Type Property

# deallocateReceiveRight

Remove a receive right when the `NSMachPort` object is invalidated or destroyed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var deallocateReceiveRight: NSMachPort.Options { get }
```

## See Also

### Constants

static var deallocateSendRight: NSMachPort.Options

Deallocate a send right when the `NSMachPort` object is invalidated or destroyed.

