

- UIKit
- UIColorPickerViewControllerDelegate
-  colorPickerViewControllerDidSelectColor(\_:) Deprecated

Instance Method

# colorPickerViewControllerDidSelectColor(\_:)

Informs the delegate when the user selects a color.

iOS 14.0–15.0DeprecatediPadOS 14.0–15.0DeprecatedMac Catalyst 14.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
optional func colorPickerViewControllerDidSelectColor(_ viewController: UIColorPickerViewController)
```

Deprecated

Use colorPickerViewController(_:didSelect:continuously:) instead.

## Parameters 

`viewController`  

The view controller that receives the color change.

