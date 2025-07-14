

- Network
- NWConnection
-  pathUpdateHandler 

Instance Property

# pathUpdateHandler

A handler that receives network path updates.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@preconcurrency
final var pathUpdateHandler: ((NWPath) -> Void)? { get set }
```

## See Also

### Handling Path Updates

var currentPath: NWPath?

The network path the connection is using.

var viabilityUpdateHandler: ((Bool) -> Void)?

A handler that receives updates when data can be sent and received.

var betterPathUpdateHandler: ((Bool) -> Void)?

A handler that receives updates when an alternative network path is preferred over the current path.

