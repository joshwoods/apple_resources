

- GameKit
- GKPeerPickerControllerDelegate
-  peerPickerControllerDidCancel(\_:) Deprecated

Instance Method

# peerPickerControllerDidCancel(\_:)

Tells the delegate that the user canceled the connection attempt.

visionOS 1.0–1.0Deprecated

``` source
optional func peerPickerControllerDidCancel(_ picker: GKPeerPickerController)
```

Deprecated

Use MCBrowserViewController along with MCBrowserViewControllerDelegate from the MultipeerConnectivity framework.

## Parameters 

`picker`  

The controller for the peer picker dialog.

## Discussion

After this method returns, the controller dismisses the picker interface.

Important

Although optional in the protocol, Game Kit expects your application to implement this method.

