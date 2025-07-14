

- UIKit
- UIActionSheetDelegate
-  actionSheet(\_:willDismissWithButtonIndex:) Deprecated

Instance Method

# actionSheet(\_:willDismissWithButtonIndex:)

Sent to the delegate before an action sheet is dismissed.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func actionSheet(
    _ actionSheet: UIActionSheet,
    willDismissWithButtonIndex buttonIndex: Int
)
```

## Parameters 

`actionSheet`  

The action sheet that is about to be dismissed.

`buttonIndex`  

The index of the button that was clicked. If this is the cancel button index, the action sheet is canceling. If `-1`, the cancel button index is not set.

## Discussion

This method is invoked before the animation begins and the view is hidden.

## See Also

### Customizing behavior

func willPresent(UIActionSheet)

Sent to the delegate before an action sheet is presented to the user.

Deprecated

func didPresent(UIActionSheet)

Sent to the delegate after an action sheet is presented to the user.

Deprecated

func actionSheet(UIActionSheet, didDismissWithButtonIndex: Int)

Sent to the delegate after an action sheet is dismissed from the screen.

Deprecated

