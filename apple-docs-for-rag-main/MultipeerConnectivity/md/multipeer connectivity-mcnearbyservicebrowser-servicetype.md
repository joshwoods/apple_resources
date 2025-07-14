

- Multipeer Connectivity
- MCNearbyServiceBrowser
-  serviceType 

Instance Property

# serviceType

The service type to browse for.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
var serviceType: String { get }
```

## Discussion

This value is set when you initialize the object, and cannot be changed later.

## See Also

### Initializing the Browser

init(peer: MCPeerID, serviceType: String)

Initializes the nearby service browser object.

var delegate: (any MCNearbyServiceBrowserDelegate)?

The delegate object that handles browser-related events.

var myPeerID: MCPeerID

The local peer ID for this instance.

