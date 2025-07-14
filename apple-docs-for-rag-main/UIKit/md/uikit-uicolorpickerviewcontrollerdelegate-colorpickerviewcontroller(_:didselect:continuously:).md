

- UIKit
- UIColorPickerViewControllerDelegate
-  colorPickerViewController(\_:didSelect:continuously:) 

Instance Method

# colorPickerViewController(\_:didSelect:continuously:)

Informs the delegate when a user selects a color, indicating whether the update is part of a continuous user interaction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
optional func colorPickerViewController(
    _ viewController: UIColorPickerViewController,
    didSelect color: UIColor,
    continuously: Bool
)
```

## Parameters 

`viewController`  

The color picker.

`color`  

The new color.

`continuously`  

A Boolean value that indicates whether the update is part of a continuous user interaction.

## Discussion

A continuous selection is always followed by a noncontinuous one when the user finishes the gesture. Apps that support undoing should update their UI for all color changes but only undo to noncontinuous color changes.

## See Also

### Handling color picker activity

func colorPickerViewControllerDidFinish(UIColorPickerViewController)

Informs the delegate that the user dismissed the color picker.

