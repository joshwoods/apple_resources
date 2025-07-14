

- Multipeer Connectivity
- MCSession
-  myPeerID 

Instance Property

# myPeerID

A local identifier that represents the device on which your app is currently running.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
var myPeerID: MCPeerID { get }
```

## Discussion

You set this value when you initialize the session object. It cannot be changed later.

## See Also

### Creating a Session

convenience init(peer: MCPeerID)

Creates a Multipeer Connectivity session.

init(peer: MCPeerID, securityIdentity: [Any]?, encryptionPreference: MCEncryptionPreference)

Creates a Multipeer Connectivity session, providing security information.

var delegate: (any MCSessionDelegate)?

The delegate object that handles session-related events.

var encryptionPreference: MCEncryptionPreference

A value indicating whether the connection prefers encrypted connections, unencrypted connections, or has no preference.

var securityIdentity: [Any]?

The security identity of the local peer.

