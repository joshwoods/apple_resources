

- GameKit
- GKPeerPickerControllerDelegate
-  peerPickerController(\_:didConnectPeer:to:) Deprecated

Instance Method

# peerPickerController(\_:didConnectPeer:to:)

Tells the delegate that the controller connected a peer to the session.

visionOS 1.0–1.0Deprecated

``` source
optional func peerPickerController(
    _ picker: GKPeerPickerController,
    didConnectPeer peerID: String,
    to session: GKSession
)
```

Deprecated

Use MCBrowserViewController along with MCBrowserViewControllerDelegate from the MultipeerConnectivity framework.

## Parameters 

`picker`  

The controller that connected the peer.

`peerID`  

The identification string for the peer that connected to the session.

`session`  

The session that the peer is connected to.

## Discussion

Once a peer is connected to the session, your application should take ownership of the session, dismiss the peer picker, and then use the session to communicate with the other peer.

Important

Although optional in the protocol, Game Kit expects your application to implement this method.

