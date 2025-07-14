

- UIKit
- UIAlertView
-  dismiss(withClickedButtonIndex:animated:) Deprecated

Instance Method

# dismiss(withClickedButtonIndex:animated:)

Dismisses the receiver, optionally with animation.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func dismiss(
    withClickedButtonIndex buttonIndex: Int,
    animated: Bool
)
```

## Parameters 

`buttonIndex`  

The index of the button that was clicked just before invoking this method. The button indices start at `0`.

`animated`  

true if the receiver should be removed by animating it first; otherwise, false if it should be removed immediately with no animation.

## Discussion

In iOS 4.0, you may want to call this method whenever your application moves to the background. An alert view is not dismissed automatically when an application moves to the background. This behavior differs from previous versions of the operating system, where they were canceled automatically when the application was terminated. Dismissing the alert view gives your application a chance to save changes or abort the operation and perform any necessary cleanup in case your application is terminated later.

