

- ARKit
- ARSession
- ARSession.CollaborationData
-  ARSession.CollaborationData.Priority 

Enumeration

# ARSession.CollaborationData.Priority

Options that help you choose the appropriate network protocol or settings for a given data instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum Priority
```

## Discussion

When you send ARSession.CollaborationData over the network by using a protocol that allows you to specify varying reliability, this property provides you with a hint about which reliability setting to use for a given collaboration data instance. Depending on its priority, you may also choose to send a given collaboration data instance using different protocols.

## Topics

### Enumeration Cases

case critical

A priority that indicates that collaboration depends on this data.

case optional

A priority that indicates that collaboration can continue without this data.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Observing Priority

var priority: ARSession.CollaborationData.Priority

A property that gives you a hint about how to send a given data instance over the network.

