

- UIKit
- UIFontPickerViewController
-  selectedFontDescriptor 

Instance Property

# selectedFontDescriptor

Information about the font family or face selected by the user in the font picker.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var selectedFontDescriptor: UIFontDescriptor? { get set }
```

## Discussion

This font descriptor does not include a size attribute, so if you want to use this descriptor as a parameter in init(descriptor:size:), you also need a size parameter greater than `0.0`.

## See Also

### Responding to font picker interactions

var delegate: (any UIFontPickerViewControllerDelegate)?

The object that handles messages about the user’s interaction with a font picker.

protocol UIFontPickerViewControllerDelegate

A set of optional methods for receiving messages about the user’s interaction with the font picker.

