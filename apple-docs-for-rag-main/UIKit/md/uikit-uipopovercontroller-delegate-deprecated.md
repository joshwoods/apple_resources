

- UIKit
- UIPopoverController
-  delegate Deprecated

Instance Property

# delegate

The delegate you want to receive popover controller messages.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
weak var delegate: (any UIPopoverControllerDelegate)? { get set }
```

## Discussion

The popover controller uses its delegate to determine whether it should dismiss the popover and provides a notification when such an event occurs. For more information about the methods you can implement in your delegate, see UIPopoverControllerDelegate.

