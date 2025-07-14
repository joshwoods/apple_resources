

- UIKit
-  UIFontPickerViewControllerDelegate 

Protocol

# UIFontPickerViewControllerDelegate

A set of optional methods for receiving messages about the user’s interaction with the font picker.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIFontPickerViewControllerDelegate : NSObjectProtocol
```

## Topics

### Receiving font picker interactions

func fontPickerViewControllerDidCancel(UIFontPickerViewController)

Tells the delegate that the user dismissed the font picker without selecting a font.

func fontPickerViewControllerDidPickFont(UIFontPickerViewController)

Tells the delegate that the user has selected a font.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UITextFormattingCoordinator

## See Also

### Font picker

class UIFontPickerViewController

A view controller that manages the interface for selecting a font that the system provides or the user installs.

class Configuration

The filters and display settings a font picker view controller uses to set up a font picker.

