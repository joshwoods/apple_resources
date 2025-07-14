

- Network
- NWListener
-  InfiniteConnectionLimit 

Type Property

# InfiniteConnectionLimit

A static value to indicate that inbound connections should not be limited.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let InfiniteConnectionLimit: Int
```

## See Also

### Receiving Connections

var newConnectionHandler: ((NWConnection) -> Void)?

A handler that receives inbound connections.

var newConnectionLimit: Int

The remaining number of inbound connections to deliver before rejecting connections.

