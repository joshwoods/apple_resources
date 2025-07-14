

- Foundation
- PortMessage
-  receivePort 

Instance Property

# receivePort

For an outgoing message, returns the port on which replies to the receiver will arrive. For an incoming message, returns the port the receiver did arrive on.

Mac Catalyst 13.0+macOS 10.0+

``` source
var receivePort: Port? { get }
```

## Return Value

For an outgoing message, the port on which replies to the receiver will arrive. For an incoming message, the port the receiver did arrive on.

## See Also

### Getting the Ports

var sendPort: Port?

For an outgoing message, returns the port the receiver will send itself through. For an incoming message, returns the port replies to the receiver should be sent through.

