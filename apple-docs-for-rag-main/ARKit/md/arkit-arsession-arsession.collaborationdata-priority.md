

- ARKit
- ARSession
- ARSession.CollaborationData
-  priority 

Instance Property

# priority

A property that gives you a hint about how to send a given data instance over the network.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var priority: ARSession.CollaborationData.Priority { get }
```

## Discussion

If you have reliability options in the network protocol you choose to transport ARSession.CollaborationData among peers, the priority property gives you a hint about which reliability option to choose for a given collaboration data instance. For example, if you use MultipeerConnectivity to send collaboration data over the network, choose MCSessionSendDataMode.reliable when calling send(_:toPeers:with:) after ARKit gives you a collaboration data instance with priority ARSession.CollaborationData.Priority.critical.

## See Also

### Observing Priority

enum Priority

Options that help you choose the appropriate network protocol or settings for a given data instance.

