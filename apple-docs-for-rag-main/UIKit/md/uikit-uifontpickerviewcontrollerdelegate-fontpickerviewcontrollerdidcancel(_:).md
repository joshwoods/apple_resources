

- UIKit
- UIFontPickerViewControllerDelegate
-  fontPickerViewControllerDidCancel(\_:) 

Instance Method

# fontPickerViewControllerDidCancel(\_:)

Tells the delegate that the user dismissed the font picker without selecting a font.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func fontPickerViewControllerDidCancel(_ viewController: UIFontPickerViewController)
```

## Parameters 

`viewController`  

The controller for the font picker that was canceled.

## Discussion

Implement this optional method if your app needs to add custom logic when the user cancels the font picker instead of picking a font.

## See Also

### Receiving font picker interactions

func fontPickerViewControllerDidPickFont(UIFontPickerViewController)

Tells the delegate that the user has selected a font.

