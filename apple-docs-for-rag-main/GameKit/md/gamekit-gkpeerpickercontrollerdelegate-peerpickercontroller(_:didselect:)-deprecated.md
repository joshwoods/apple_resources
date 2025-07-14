

- GameKit
- GKPeerPickerControllerDelegate
-  peerPickerController(\_:didSelect:) Deprecated

Instance Method

# peerPickerController(\_:didSelect:)

Tells the delegate that the user selected a connection type.

visionOS 1.0–1.0Deprecated

``` source
optional func peerPickerController(
    _ picker: GKPeerPickerController,
    didSelect type: GKPeerPickerConnectionType
)
```

Deprecated

Use MCBrowserViewController along with MCBrowserViewControllerDelegate from the MultipeerConnectivity framework.

## Parameters 

`picker`  

The controller for the peer picker dialog.

`type`  

The type of network connection chosen by the user.

## Discussion

If the peer picker is configured to allow users to choose between multiple connection types, this method is called when users select the connection type they want to use. Your delegate implements this method if you want to override the behavior for a particular connection type.

Important

In iOS 3.0, the peer picker can configure Bluetooth connections (GKPeerPickerConnectionType.nearby). If the user chooses an Internet connection (GKPeerPickerConnectionType.online), your delegate should dismiss the dialog and present its own user interface to configure the Internet connection:

```
- (void)peerPickerController:(GKPeerPickerController *)picker didSelectConnectionType:(GKPeerPickerConnectionType)type {
    if(type == GKPeerPickerConnectionTypeOnline) {
        [picker dismiss];
        [picker autorelease];
// Display your own user interface here.
}
```

## See Also

### Creating a Session for the Peer Picker

func peerPickerController(GKPeerPickerController, sessionFor: GKPeerPickerConnectionType) -> GKSession

Asks the delegate to return a session for the specified connection type.

Deprecated

