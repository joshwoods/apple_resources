

- Multipeer Connectivity
- MCSession
-  delegate 

Instance Property

# delegate

The delegate object that handles session-related events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
weak var delegate: (any MCSessionDelegate)? { get set }
```

## See Also

### Creating a Session

convenience init(peer: MCPeerID)

Creates a Multipeer Connectivity session.

init(peer: MCPeerID, securityIdentity: [Any]?, encryptionPreference: MCEncryptionPreference)

Creates a Multipeer Connectivity session, providing security information.

var encryptionPreference: MCEncryptionPreference

A value indicating whether the connection prefers encrypted connections, unencrypted connections, or has no preference.

var myPeerID: MCPeerID

A local identifier that represents the device on which your app is currently running.

var securityIdentity: [Any]?

The security identity of the local peer.

