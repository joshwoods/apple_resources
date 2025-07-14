

- UIKit
- UIColorPickerViewController
-  supportsAlpha 

Instance Property

# supportsAlpha

A Boolean value that enables alpha value control.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var supportsAlpha: Bool { get set }
```

## See Also

### Configuring the color picker view controller

var delegate: (any UIColorPickerViewControllerDelegate)?

The delegate that receives updates about the color selection.

protocol UIColorPickerViewControllerDelegate

The delegate protocol to inform about changes in color selection.

var selectedColor: UIColor

The color selected by the user.

