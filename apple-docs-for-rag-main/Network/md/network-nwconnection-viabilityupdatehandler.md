

- Network
- NWConnection
-  viabilityUpdateHandler 

Instance Property

# viabilityUpdateHandler

A handler that receives updates when data can be sent and received.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@preconcurrency
final var viabilityUpdateHandler: ((Bool) -> Void)? { get set }
```

## See Also

### Handling Path Updates

var currentPath: NWPath?

The network path the connection is using.

var pathUpdateHandler: ((NWPath) -> Void)?

A handler that receives network path updates.

var betterPathUpdateHandler: ((Bool) -> Void)?

A handler that receives updates when an alternative network path is preferred over the current path.

