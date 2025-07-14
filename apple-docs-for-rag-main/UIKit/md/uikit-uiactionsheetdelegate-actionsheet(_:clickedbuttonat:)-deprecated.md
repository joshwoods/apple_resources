

- UIKit
- UIActionSheetDelegate
-  actionSheet(\_:clickedButtonAt:) Deprecated

Instance Method

# actionSheet(\_:clickedButtonAt:)

Sent to the delegate when the user clicks a button on an action sheet.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func actionSheet(
    _ actionSheet: UIActionSheet,
    clickedButtonAt buttonIndex: Int
)
```

## Parameters 

`actionSheet`  

The action sheet containing the button.

`buttonIndex`  

The position of the clicked button. The button indices start at `0`.

## Discussion

The receiver is automatically dismissed after this method is invoked.

