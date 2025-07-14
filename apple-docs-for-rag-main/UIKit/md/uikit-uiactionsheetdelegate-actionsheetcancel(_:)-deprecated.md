

- UIKit
- UIActionSheetDelegate
-  actionSheetCancel(\_:) Deprecated

Instance Method

# actionSheetCancel(\_:)

Sent to the delegate before an action sheet is canceled.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func actionSheetCancel(_ actionSheet: UIActionSheet)
```

## Parameters 

`actionSheet`  

The action sheet that will be canceled.

## Discussion

If the action sheet’s delegate does not implement this method, clicking the cancel button is simulated and the action sheet is dismissed. Implement this method if you need to perform some actions before an action sheet is canceled. An action sheet can be canceled at any time by the system—for example, when the user taps the Home button. The actionSheet(_:willDismissWithButtonIndex:) and actionSheet(_:didDismissWithButtonIndex:) methods are invoked after this method.

