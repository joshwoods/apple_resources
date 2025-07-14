

- UIKit
- UIColorPickerViewControllerDelegate
-  colorPickerViewControllerDidFinish(\_:) 

Instance Method

# colorPickerViewControllerDidFinish(\_:)

Informs the delegate that the user dismissed the color picker.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
optional func colorPickerViewControllerDidFinish(_ viewController: UIColorPickerViewController)
```

## Parameters 

`viewController`  

The view controller that starts dismissing.

## Discussion

The system calls this method when the user dismisses the color picker.

You can implement this method to show additional animations alongside the dismissal animation. For interactive dismissals, use the delegate of the presentation controller that manages the color picker instead.

## See Also

### Handling color picker activity

func colorPickerViewController(UIColorPickerViewController, didSelect: UIColor, continuously: Bool)

Informs the delegate when a user selects a color, indicating whether the update is part of a continuous user interaction.

