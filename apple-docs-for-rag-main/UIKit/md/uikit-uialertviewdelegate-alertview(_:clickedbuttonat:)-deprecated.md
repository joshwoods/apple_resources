

- UIKit
- UIAlertViewDelegate
-  alertView(\_:clickedButtonAt:) Deprecated

Instance Method

# alertView(\_:clickedButtonAt:)

Sent to the delegate when the user clicks a button on an alert view.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func alertView(
    _ alertView: UIAlertView,
    clickedButtonAt buttonIndex: Int
)
```

## Parameters 

`alertView`  

The alert view containing the button.

`buttonIndex`  

The index of the button that was clicked. The button indices start at `0`.

## Discussion

The receiver is automatically dismissed after this method is invoked.

