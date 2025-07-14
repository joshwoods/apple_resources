

- UIKit
- UIColorPickerViewController
-  selectedColor 

Instance Property

# selectedColor

The color selected by the user.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var selectedColor: UIColor { get set }
```

## See Also

### Configuring the color picker view controller

var delegate: (any UIColorPickerViewControllerDelegate)?

The delegate that receives updates about the color selection.

protocol UIColorPickerViewControllerDelegate

The delegate protocol to inform about changes in color selection.

var supportsAlpha: Bool

A Boolean value that enables alpha value control.

