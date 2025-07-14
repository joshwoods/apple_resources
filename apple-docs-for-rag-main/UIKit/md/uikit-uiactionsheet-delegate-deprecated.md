

- UIKit
- UIActionSheet
-  delegate Deprecated

Instance Property

# delegate

The receiver’s delegate or `nil` if it doesn’t have a delegate.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
weak var delegate: (any UIActionSheetDelegate)? { get set }
```

## Discussion

For a list of methods your delegate object can implement, see UIActionSheetDelegate.

## See Also

### Setting properties

var title: String

The string that appears in the receiver’s title bar.

Deprecated

var isVisible: Bool

A Boolean value that indicates whether the receiver is displayed.

Deprecated

var actionSheetStyle: UIActionSheetStyle

The receiver’s presentation style.

Deprecated

