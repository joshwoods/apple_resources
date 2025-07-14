

- UIKit
-  UIColorPickerViewController 

Class

# UIColorPickerViewController

A view controller that manages the interface for selecting a color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
class UIColorPickerViewController
```

## Overview

UIColorPickerViewController provides a standard interface to select colors. Use this class instead of UIColorWell if you need more fine-grained control over the presentation.

You typically present a UIColorPickerViewController as a popover:

```
// This example code appears in a subclass of UIViewController that conforms to
// UIColorPickerViewControllerDelegate.
func presentColorPicker() {
    let colorPicker = UIColorPickerViewController()
    colorPicker.title = "Background Color"
    colorPicker.supportsAlpha = false
    colorPicker.delegate = self
    colorPicker.modalPresentationStyle = .popover
    colorPicker.popoverPresentationController?.sourceItem = self.navigationItem.rightBarButtonItem
    self.present(colorPicker, animated: true)
}
```

You can also react to the color-selection change or the dismissal of the color picker by implementing the UIColorPickerViewControllerDelegate functions.

## Topics

### Creating a color picker view controller

init()

Creates a color picker view controller.

### Configuring the color picker view controller

var delegate: (any UIColorPickerViewControllerDelegate)?

The delegate that receives updates about the color selection.

protocol UIColorPickerViewControllerDelegate

The delegate protocol to inform about changes in color selection.

var selectedColor: UIColor

The color selected by the user.

var supportsAlpha: Bool

A Boolean value that enables alpha value control.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Color picker

protocol UIColorPickerViewControllerDelegate

The delegate protocol to inform about changes in color selection.

