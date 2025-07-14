

- UIKit
- UIPreviewAction
-  handler Deprecated

Instance Property

# handler

The block called when the peek quick action is selected by the user.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
var handler: (any UIPreviewActionItem, UIViewController) -> Void { get }
```

## Discussion

The handler is set when the peek quick action is instantiated; it is immutable.

## See Also

### Creating a peek quick action

convenience init(title: String, style: UIPreviewAction.Style, handler: (UIPreviewAction, UIViewController) -> Void)

Creates a peek quick action using a specified title, style, and handler.

Deprecated

enum Style

The style for a peek quick action.

Deprecated

