

- GameKit
- GKPeerPickerController
-  connectionTypesMask Deprecated

Instance Property

# connectionTypesMask

A mask that determines the types of connections a dialog presents to the user.

visionOS 1.0–1.0Deprecated

``` source
var connectionTypesMask: GKPeerPickerConnectionType { get set }
```

Deprecated

Use MCBrowserViewController from the MultipeerConnectivity framework.

## Discussion

Your application configures the connection types it allows before showing the peer picker. If your application allows more than one connection type, the peer picker offers the user a choice of which type of connection to use. The default value for the mask is GKPeerPickerConnectionType.nearby.

Important

In iOS 3.0, GKPeerPickerConnectionType.nearby is required to be one of the allowed connection types. An exception is thrown if your application does not include it.

