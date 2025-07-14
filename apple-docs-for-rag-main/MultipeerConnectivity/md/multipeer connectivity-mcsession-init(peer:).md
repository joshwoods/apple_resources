

- Multipeer Connectivity
- MCSession
-  init(peer:) 

Initializer

# init(peer:)

Creates a Multipeer Connectivity session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
convenience init(peer myPeerID: MCPeerID)
```

## Parameters 

`myPeerID`  

A local identifier that represents the device on which your app is currently running.

## Return Value

The initialized session object, or `nil` if an error occurs.

## Discussion

This method is equivalent to calling init(peer:securityIdentity:encryptionPreference:) with a `nil` identity and an encryption setting that varies based on which version of the SDK was used to link the application. On apps linked on or after iOS 9, the encryption is set to MCEncryptionPreference.required. On apps linked prior to iOS 9, the encryption is set to MCEncryptionPreference.optional.

This method throws an exception if the provided peer ID object is invalid or `nil`.

For more information, see Initiating a Session.

## See Also

### Creating a Session

init(peer: MCPeerID, securityIdentity: [Any]?, encryptionPreference: MCEncryptionPreference)

Creates a Multipeer Connectivity session, providing security information.

var delegate: (any MCSessionDelegate)?

The delegate object that handles session-related events.

var encryptionPreference: MCEncryptionPreference

A value indicating whether the connection prefers encrypted connections, unencrypted connections, or has no preference.

var myPeerID: MCPeerID

A local identifier that represents the device on which your app is currently running.

var securityIdentity: [Any]?

The security identity of the local peer.

