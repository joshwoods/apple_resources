

- UIKit
- UIAlertViewDelegate
-  alertView(\_:didDismissWithButtonIndex:) Deprecated

Instance Method

# alertView(\_:didDismissWithButtonIndex:)

Sent to the delegate after an alert view is dismissed from the screen.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func alertView(
    _ alertView: UIAlertView,
    didDismissWithButtonIndex buttonIndex: Int
)
```

## Parameters 

`alertView`  

The alert view that was dismissed.

`buttonIndex`  

The index of the button that was clicked. The button indices start at `0`. If this is the cancel button index, the alert view is canceling. If `-1`, the cancel button index is not set.

## Discussion

This method is invoked after the animation ends and the view is hidden.

## See Also

### Customizing behavior

func alertViewShouldEnableFirstOtherButton(UIAlertView) -> Bool

Sent to the delegate to determine whether the first non-cancel button in the alert should be enabled.

Deprecated

func willPresent(UIAlertView)

Sent to the delegate before a model view is presented to the user.

Deprecated

func didPresent(UIAlertView)

Sent to the delegate after an alert view is presented to the user.

Deprecated

func alertView(UIAlertView, willDismissWithButtonIndex: Int)

Sent to the delegate before an alert view is dismissed.

Deprecated

