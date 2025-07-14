

- GameKit
- GKDialogController
-  parentWindow 

Instance Property

# parentWindow

The window that displays the dashboard.

macOS 10.8+

``` source
@IBOutlet @MainActor
weak var parentWindow: NSWindow? { get set }
```

## Discussion

Set this property before presenting a view controller. The window must be at least 800 x 600.

