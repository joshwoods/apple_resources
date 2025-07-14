

- UIKit
- UIAlertViewDelegate
-  alertViewCancel(\_:) Deprecated

Instance Method

# alertViewCancel(\_:)

Sent to the delegate before an alert view is canceled.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func alertViewCancel(_ alertView: UIAlertView)
```

## Parameters 

`alertView`  

The alert view that will be canceled.

## Discussion

If the alert view’s delegate does not implement this method, clicking the cancel button is simulated and the alert view is dismissed. Implement this method if you need to perform some actions before an alert view is canceled. An alert view can be canceled at any time by the system—for example, when the user taps the Home button. The alertView(_:willDismissWithButtonIndex:) and alertView(_:didDismissWithButtonIndex:) methods are invoked after this method.

