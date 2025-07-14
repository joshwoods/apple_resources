

- UIKit
-  UIColorPickerViewControllerDelegate 

Protocol

# UIColorPickerViewControllerDelegate

The delegate protocol to inform about changes in color selection.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
protocol UIColorPickerViewControllerDelegate : NSObjectProtocol
```

## Overview

By implementing the UIColorPickerViewControllerDelegate functions, your app can react to a color-selection change or the dismissal of the color picker.

## Topics

### Handling color picker activity

func colorPickerViewControllerDidFinish(UIColorPickerViewController)

Informs the delegate that the user dismissed the color picker.

func colorPickerViewController(UIColorPickerViewController, didSelect: UIColor, continuously: Bool)

Informs the delegate when a user selects a color, indicating whether the update is part of a continuous user interaction.

### Deprecated

func colorPickerViewControllerDidSelectColor(UIColorPickerViewController)

Informs the delegate when the user selects a color.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Color picker

class UIColorPickerViewController

A view controller that manages the interface for selecting a color.

