

- GameKit
- GKPeerPickerControllerDelegate
-  peerPickerController(\_:sessionFor:) Deprecated

Instance Method

# peerPickerController(\_:sessionFor:)

Asks the delegate to return a session for the specified connection type.

visionOS 1.0–1.0Deprecated

``` source
optional func peerPickerController(
    _ picker: GKPeerPickerController,
    sessionFor type: GKPeerPickerConnectionType
) -> GKSession
```

Deprecated

Use MCBrowserViewController along with MCBrowserViewControllerDelegate from the MultipeerConnectivity framework.

## Parameters 

`picker`  

The controller requesting the session.

`type`  

The type of connection the controller wants to configure.

## Discussion

Your delegate is responsible for providing a GKSession to use to find and connect to other devices. When the peer picker needs a session, it calls this method. Your application can either create a new session or return a previously created session to the peer picker. The session that your application returns to the peer picker must advertise itself as a peer (GKSessionMode.peer).

If your delegate does not implement this method and the user selected a network of type GKPeerPickerConnectionType.nearby, the peer controller allocates a new session that advertises itself as a peer (GKSessionMode.peer) with the default sessionID and displayName parameters.

### Special Considerations

In iOS 3.0, your delegate receives requests only for networks of type GKPeerPickerConnectionType.nearby.

## See Also

### Creating a Session for the Peer Picker

func peerPickerController(GKPeerPickerController, didSelect: GKPeerPickerConnectionType)

Tells the delegate that the user selected a connection type.

Deprecated

