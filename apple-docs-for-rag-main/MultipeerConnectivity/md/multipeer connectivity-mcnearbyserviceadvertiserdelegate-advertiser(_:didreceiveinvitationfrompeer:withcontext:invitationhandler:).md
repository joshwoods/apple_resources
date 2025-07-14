

- Multipeer Connectivity
- MCNearbyServiceAdvertiserDelegate
-  advertiser(\_:didReceiveInvitationFromPeer:withContext:invitationHandler:) 

Instance Method

# advertiser(\_:didReceiveInvitationFromPeer:withContext:invitationHandler:)

Called when an invitation to join a session is received from a nearby peer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func advertiser(
    _ advertiser: MCNearbyServiceAdvertiser,
    didReceiveInvitationFromPeer peerID: MCPeerID,
    withContext context: Data?,
    invitationHandler: @escaping (Bool, MCSession?) -> Void
)
```

**Required**

## Parameters 

`advertiser`  

The advertiser object that was invited to join the session.

`peerID`  

The peer ID of the nearby peer that invited your app to join the session.

`context`  

An arbitrary piece of data received from the nearby peer. This can be used to provide further information to the user about the nature of the invitation.

Important

The nearby peer should treat any data it receives as potentially untrusted. To learn more about working with untrusted data, read Secure Coding Guide.

`invitationHandler`  

A block that your code must call to indicate whether the advertiser should accept or decline the invitation, and to provide a session with which to associate the peer that sent the invitation.

