

- UIKit
- UIActionSheetDelegate
-  actionSheet(\_:didDismissWithButtonIndex:) Deprecated

Instance Method

# actionSheet(\_:didDismissWithButtonIndex:)

Sent to the delegate after an action sheet is dismissed from the screen.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func actionSheet(
    _ actionSheet: UIActionSheet,
    didDismissWithButtonIndex buttonIndex: Int
)
```

## Parameters 

`actionSheet`  

The action sheet that was dismissed.

`buttonIndex`  

The index of the button that was clicked. The button indices start at `0`. If this is the cancel button index, the action sheet is canceling. If `-1`, the cancel button index is not set.

## Discussion

This method is invoked after the animation ends and the view is hidden.

## See Also

### Customizing behavior

func willPresent(UIActionSheet)

Sent to the delegate before an action sheet is presented to the user.

Deprecated

func didPresent(UIActionSheet)

Sent to the delegate after an action sheet is presented to the user.

Deprecated

func actionSheet(UIActionSheet, willDismissWithButtonIndex: Int)

Sent to the delegate before an action sheet is dismissed.

Deprecated

