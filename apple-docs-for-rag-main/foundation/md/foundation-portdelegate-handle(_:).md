

- Foundation
- PortDelegate
-  handle(\_:) 

Instance Method

# handle(\_:)

Processes a given incoming message on the port.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
optional func handle(_ message: NSPortMessage)
```

**Mac Catalyst, macOS**

``` source
optional func handle(_ message: PortMessage)
```

## Parameters 

`message`  

An incoming port message.

## Discussion

See Port for more information.

The delegate should implement either handle(_:) or the NSMachPortDelegate protocol method handleMachMessage(_:). You must not implement both delegate methods.

## See Also

### Related Documentation

Distributed Objects Programming Topics

