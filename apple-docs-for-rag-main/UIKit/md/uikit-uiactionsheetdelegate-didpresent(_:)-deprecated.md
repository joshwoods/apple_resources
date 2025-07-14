

- UIKit
- UIActionSheetDelegate
-  didPresent(\_:) Deprecated

Instance Method

# didPresent(\_:)

Sent to the delegate after an action sheet is presented to the user.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func didPresent(_ actionSheet: UIActionSheet)
```

## Parameters 

`actionSheet`  

The action sheet that was displayed.

## See Also

### Customizing behavior

func willPresent(UIActionSheet)

Sent to the delegate before an action sheet is presented to the user.

Deprecated

func actionSheet(UIActionSheet, willDismissWithButtonIndex: Int)

Sent to the delegate before an action sheet is dismissed.

Deprecated

func actionSheet(UIActionSheet, didDismissWithButtonIndex: Int)

Sent to the delegate after an action sheet is dismissed from the screen.

Deprecated

