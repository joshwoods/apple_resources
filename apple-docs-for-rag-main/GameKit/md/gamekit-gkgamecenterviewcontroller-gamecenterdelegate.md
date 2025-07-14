

- GameKit
- GKGameCenterViewController
-  gameCenterDelegate 

Instance Property

# gameCenterDelegate

The view controller’s delegate.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
weak var gameCenterDelegate: (any GKGameCenterControllerDelegate)? { get set }
```

## Discussion

Before presenting the view controller, your game must set a delegate.

## See Also

### Setting the view controller delegate

protocol GKGameCenterControllerDelegate

The delegate that GameKit calls when the player dismisses the dashboard.

