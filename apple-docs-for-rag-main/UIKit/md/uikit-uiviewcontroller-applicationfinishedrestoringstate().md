

- UIKit
- UIViewController
-  applicationFinishedRestoringState() 

Instance Method

# applicationFinishedRestoringState()

Called on restored view controllers after other object decoding is complete.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func applicationFinishedRestoringState()
```

## Discussion

After other object decoding has completed, the system calls this method. This allows a view controller to complete setup after other state restoration, relying on the system to ensure that the states of all objects from the restoration archive have been decoded.

## See Also

### Managing state restoration

Restoring your app’s state

Provide continuity for the user by preserving current activities.

var restorationIdentifier: String?

The identifier that determines whether the view controller supports state restoration.

var restorationClass: (any UIViewControllerRestoration.Type)?

The class responsible for recreating this view controller when restoring the app’s state.

func encodeRestorableState(with: NSCoder)

Encodes state-related information for the view controller.

func decodeRestorableState(with: NSCoder)

Decodes and restores state-related information for the view controller.

