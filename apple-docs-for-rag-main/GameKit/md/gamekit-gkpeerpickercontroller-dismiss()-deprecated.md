

- GameKit
- GKPeerPickerController
-  dismiss() Deprecated

Instance Method

# dismiss()

Hides the peer picker dialog.

visionOS 1.0–1.0Deprecated

``` source
func dismiss()
```

Deprecated

Use MCBrowserViewController from the MultipeerConnectivity framework.

## Discussion

The controller’s delegate is responsible for dismissing the peer picker when it is no longer needed.

On iOS 3.1 or later, the peer picker is retained when it is shown, and autoreleased when it is dismissed.

## See Also

### Displaying the Picker Dialog

func show()

Displays the peer picker dialog to the user.

Deprecated

var isVisible: Bool

A Boolean value that indicates whether the picker dialog is visible.

Deprecated

