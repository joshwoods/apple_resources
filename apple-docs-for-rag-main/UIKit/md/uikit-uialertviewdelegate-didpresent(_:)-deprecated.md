

- UIKit
- UIAlertViewDelegate
-  didPresent(\_:) Deprecated

Instance Method

# didPresent(\_:)

Sent to the delegate after an alert view is presented to the user.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func didPresent(_ alertView: UIAlertView)
```

## Parameters 

`alertView`  

The alert view that was displayed.

## See Also

### Customizing behavior

func alertViewShouldEnableFirstOtherButton(UIAlertView) -> Bool

Sent to the delegate to determine whether the first non-cancel button in the alert should be enabled.

Deprecated

func willPresent(UIAlertView)

Sent to the delegate before a model view is presented to the user.

Deprecated

func alertView(UIAlertView, willDismissWithButtonIndex: Int)

Sent to the delegate before an alert view is dismissed.

Deprecated

func alertView(UIAlertView, didDismissWithButtonIndex: Int)

Sent to the delegate after an alert view is dismissed from the screen.

Deprecated

