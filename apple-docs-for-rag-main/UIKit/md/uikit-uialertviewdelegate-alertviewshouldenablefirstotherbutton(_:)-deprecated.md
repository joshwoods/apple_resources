

- UIKit
- UIAlertViewDelegate
-  alertViewShouldEnableFirstOtherButton(\_:) Deprecated

Instance Method

# alertViewShouldEnableFirstOtherButton(\_:)

Sent to the delegate to determine whether the first non-cancel button in the alert should be enabled.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func alertViewShouldEnableFirstOtherButton(_ alertView: UIAlertView) -> Bool
```

## Parameters 

`alertView`  

The alert view that is being configured.

## Return Value

true if the button should be enabled, no if the button should be disabled.

## See Also

### Customizing behavior

func willPresent(UIAlertView)

Sent to the delegate before a model view is presented to the user.

Deprecated

func didPresent(UIAlertView)

Sent to the delegate after an alert view is presented to the user.

Deprecated

func alertView(UIAlertView, willDismissWithButtonIndex: Int)

Sent to the delegate before an alert view is dismissed.

Deprecated

func alertView(UIAlertView, didDismissWithButtonIndex: Int)

Sent to the delegate after an alert view is dismissed from the screen.

Deprecated

