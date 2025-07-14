

- Foundation
- PortMessage
-  sendPort 

Instance Property

# sendPort

For an outgoing message, returns the port the receiver will send itself through. For an incoming message, returns the port replies to the receiver should be sent through.

Mac Catalyst 13.0+macOS 10.0+

``` source
var sendPort: Port? { get }
```

## Return Value

For an outgoing message, the port the receiver will send itself through when it receives a send(before:) message. For an incoming message, the port replies to the receiver should be sent through.

## See Also

### Getting the Ports

var receivePort: Port?

For an outgoing message, returns the port on which replies to the receiver will arrive. For an incoming message, returns the port the receiver did arrive on.

