

- UIKit
-  UIFontPickerViewController 

Class

# UIFontPickerViewController

A view controller that manages the interface for selecting a font that the system provides or the user installs.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIFontPickerViewController
```

## Overview

Use a UIFontPickerViewController to provide the user access to all the fonts on their device. Directly querying UIFont provides only system fonts, but the user may have additional fonts on their device. When the user selects one of these nonsystem fonts in the font picker, the system grants your app access to the font.

The font picker has several customization options collected into a UIFontPickerViewController.Configuration object. For example, you can set includeFaces to true so that the user can select not only the font but a bold or italic face within that font family. Customize the configuration object first, then pass it as an argument in the font picker’s init(configuration:) method.

```
    func showFontPicker(_ sender: Any) {
        let fontConfig = UIFontPickerViewController.Configuration()
        fontConfig.includeFaces = true
        let fontPicker = UIFontPickerViewController(configuration: fontConfig)
        fontPicker.delegate = self
        self.present(fontPicker, animated: true, completion: nil)
    }
```

When your UIFontPickerViewControllerDelegate receives fontPickerViewControllerDidPickFont(_:), retrieve information about the user’s selected font from the font picker’s selectedFontDescriptor.

## Topics

### Configuring a font picker to display in iOS

init(configuration: UIFontPickerViewController.Configuration)

Creates a controller for a font picker view.

var configuration: UIFontPickerViewController.Configuration

Settings for fonts the font picker should offer to the user and how to display those fonts.

class Configuration

The filters and display settings a font picker view controller uses to set up a font picker.

### Responding to font picker interactions

var delegate: (any UIFontPickerViewControllerDelegate)?

The object that handles messages about the user’s interaction with a font picker.

protocol UIFontPickerViewControllerDelegate

A set of optional methods for receiving messages about the user’s interaction with the font picker.

var selectedFontDescriptor: UIFontDescriptor?

Information about the font family or face selected by the user in the font picker.

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

### Font picker

protocol UIFontPickerViewControllerDelegate

A set of optional methods for receiving messages about the user’s interaction with the font picker.

class Configuration

The filters and display settings a font picker view controller uses to set up a font picker.

