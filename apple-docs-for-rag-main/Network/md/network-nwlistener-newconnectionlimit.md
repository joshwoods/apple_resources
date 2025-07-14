

- Network
- NWListener
-  newConnectionLimit 

Instance Property

# newConnectionLimit

The remaining number of inbound connections to deliver before rejecting connections.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final var newConnectionLimit: Int { get set }
```

## Discussion

When the new connection limit is set to a non-infinite value, it will decrement for every received connection. Once the value hits zero, new connections will be queued and eventually blocked, until you raise the limit. This allows you to limit the rate of inbound connections you handle.

By default, the limit is InfiniteConnectionLimit. When the limit is infinite, it does not decrement but allows all inbound connections.

## See Also

### Receiving Connections

var newConnectionHandler: ((NWConnection) -> Void)?

A handler that receives inbound connections.

static let InfiniteConnectionLimit: Int

A static value to indicate that inbound connections should not be limited.

