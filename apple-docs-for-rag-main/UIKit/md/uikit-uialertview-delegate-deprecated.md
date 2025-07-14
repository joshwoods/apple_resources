

- UIKit
- UIAlertView
-  delegate Deprecated

Instance Property

# delegate

The receiver’s delegate or `nil` if it doesn’t have a delegate.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
weak var delegate: AnyObject? { get set }
```

## Discussion

See UIAlertViewDelegate for the methods this delegate should implement.

## See Also

### Setting properties

var alertViewStyle: UIAlertViewStyle

The kind of alert displayed to the user.

Deprecated

var title: String

The string that appears in the receiver’s title bar.

Deprecated

var message: String?

Descriptive text that provides more details than the title.

Deprecated

var isVisible: Bool

A Boolean value that indicates whether the receiver is displayed.

Deprecated

