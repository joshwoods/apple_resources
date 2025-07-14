

- Multipeer Connectivity
- MCNearbyServiceBrowser
-  myPeerID 

Instance Property

# myPeerID

The local peer ID for this instance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
var myPeerID: MCPeerID { get }
```

## Discussion

This value is set when you initialize the object, and cannot be changed later.

## See Also

### Initializing the Browser

init(peer: MCPeerID, serviceType: String)

Initializes the nearby service browser object.

var delegate: (any MCNearbyServiceBrowserDelegate)?

The delegate object that handles browser-related events.

var serviceType: String

The service type to browse for.

