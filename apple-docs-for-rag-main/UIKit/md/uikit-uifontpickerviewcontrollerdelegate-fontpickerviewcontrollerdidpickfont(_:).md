

- UIKit
- UIFontPickerViewControllerDelegate
-  fontPickerViewControllerDidPickFont(\_:) 

Instance Method

# fontPickerViewControllerDidPickFont(\_:)

Tells the delegate that the user has selected a font.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func fontPickerViewControllerDidPickFont(_ viewController: UIFontPickerViewController)
```

## Parameters 

`viewController`  

The controller for the font picker that has the user’s font selection.

## Discussion

When the user picks a font, you can retrieve information about the user’s selected font from the view controller’s selectedFontDescriptor.

## See Also

### Receiving font picker interactions

func fontPickerViewControllerDidCancel(UIFontPickerViewController)

Tells the delegate that the user dismissed the font picker without selecting a font.

