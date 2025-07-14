

- Multipeer Connectivity
- MCNearbyServiceBrowser
-  delegate 

Instance Property

# delegate

The delegate object that handles browser-related events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
weak var delegate: (any MCNearbyServiceBrowserDelegate)? { get set }
```

## See Also

### Initializing the Browser

init(peer: MCPeerID, serviceType: String)

Initializes the nearby service browser object.

var myPeerID: MCPeerID

The local peer ID for this instance.

var serviceType: String

The service type to browse for.

