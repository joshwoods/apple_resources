

- Multipeer Connectivity
- MCNearbyServiceAdvertiser
-  discoveryInfo 

Instance Property

# discoveryInfo

The `info` dictionary passed when this object was initialized.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
var discoveryInfo: [String : String]? { get }
```

## Discussion

This value is set when you initialize the object, and cannot be changed later.

## See Also

### Configuring and Initialization

init(peer: MCPeerID, discoveryInfo: [String : String]?, serviceType: String)

Initializes an advertiser object.

var delegate: (any MCNearbyServiceAdvertiserDelegate)?

The delegate object that handles advertising-related events.

var myPeerID: MCPeerID

The local peer ID for this instance.

var serviceType: String

The service type that your app is advertising

