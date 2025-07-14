

- UIKit
- UIColorPickerViewController
-  delegate 

Instance Property

# delegate

The delegate that receives updates about the color selection.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIColorPickerViewControllerDelegate)? { get set }
```

## See Also

### Configuring the color picker view controller

protocol UIColorPickerViewControllerDelegate

The delegate protocol to inform about changes in color selection.

var selectedColor: UIColor

The color selected by the user.

var supportsAlpha: Bool

A Boolean value that enables alpha value control.

