

- Multipeer Connectivity
- MCNearbyServiceAdvertiser
-  delegate 

Instance Property

# delegate

The delegate object that handles advertising-related events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
weak var delegate: (any MCNearbyServiceAdvertiserDelegate)? { get set }
```

## See Also

### Configuring and Initialization

init(peer: MCPeerID, discoveryInfo: [String : String]?, serviceType: String)

Initializes an advertiser object.

var discoveryInfo: [String : String]?

The `info` dictionary passed when this object was initialized.

var myPeerID: MCPeerID

The local peer ID for this instance.

var serviceType: String

The service type that your app is advertising

