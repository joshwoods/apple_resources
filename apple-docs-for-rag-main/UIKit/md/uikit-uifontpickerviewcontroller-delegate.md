

- UIKit
- UIFontPickerViewController
-  delegate 

Instance Property

# delegate

The object that handles messages about the user’s interaction with a font picker.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIFontPickerViewControllerDelegate)? { get set }
```

## See Also

### Responding to font picker interactions

protocol UIFontPickerViewControllerDelegate

A set of optional methods for receiving messages about the user’s interaction with the font picker.

var selectedFontDescriptor: UIFontDescriptor?

Information about the font family or face selected by the user in the font picker.

