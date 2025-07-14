

- Multipeer Connectivity
- MCNearbyServiceAdvertiser
-  init(peer:discoveryInfo:serviceType:) 

Initializer

# init(peer:discoveryInfo:serviceType:)

Initializes an advertiser object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
init(
    peer myPeerID: MCPeerID,
    discoveryInfo info: [String : String]?,
    serviceType: String
)
```

## Parameters 

`myPeerID`  

Your app’s local peer ID.

`info`  

A dictionary of key-value pairs that are made available to browsers. Each key and value must be an `NSString` object.

This data is advertised using a Bonjour TXT record, encoded according to RFC 6763 (section 6). As a result:

- The key-value pair must be no longer than 255 bytes (total) when encoded in UTF-8 format with an equals sign (`=`) between the key and the value.

- Keys cannot contain an equals sign.

For optimal performance, the total size of the keys and values in this dictionary should be no more than about 400 bytes so that the entire advertisement can fit within a single Bluetooth data packet. For details on the maximum allowable length, read Monitoring a Bonjour Service.

If the data you need to provide is too large to fit within these constraints, you should create a custom discovery class using Bonjour for discovery and your choice of networking protocols for exchanging the information.

`serviceType`  

The type of service to advertise. This should be a *short* text string that describes the app’s networking protocol, in the same format as a Bonjour service type (without the transport protocol) and meeting the restrictions of RFC 6335 (section 5.1) governing Service Name Syntax. In particular, the string:

- Must be 1–15 characters long

- Can contain only ASCII lowercase letters, numbers, and hyphens

- Must contain at least one ASCII letter

- Must not begin or end with a hyphen

- Must not contain hyphens adjacent to other hyphens.

This name should be easily distinguished from unrelated services. For example, a text chat app made by ABC company could use the service type `abc-txtchat`.

For more details, read Domain Naming Conventions.

## Return Value

Returns an initialized instance, or `nil` if an error occurred.

## Discussion

This method throws an exception if a valid `peerID` object is not provided or if the value of `serviceType` is not a legal Bonjour service type.

## See Also

### Configuring and Initialization

var delegate: (any MCNearbyServiceAdvertiserDelegate)?

The delegate object that handles advertising-related events.

var discoveryInfo: [String : String]?

The `info` dictionary passed when this object was initialized.

var myPeerID: MCPeerID

The local peer ID for this instance.

var serviceType: String

The service type that your app is advertising

