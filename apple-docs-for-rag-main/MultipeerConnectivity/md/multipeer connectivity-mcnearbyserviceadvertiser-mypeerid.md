

- Multipeer Connectivity
- MCNearbyServiceAdvertiser
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

### Configuring and Initialization

init(peer: MCPeerID, discoveryInfo: [String : String]?, serviceType: String)

Initializes an advertiser object.

var delegate: (any MCNearbyServiceAdvertiserDelegate)?

The delegate object that handles advertising-related events.

var discoveryInfo: [String : String]?

The `info` dictionary passed when this object was initialized.

var serviceType: String

The service type that your app is advertising

