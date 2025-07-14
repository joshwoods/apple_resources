

- UIKit
-  UITextFormattingCoordinator 

Class

# UITextFormattingCoordinator

An object that coordinates text formatting using the standard Mac font panel.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UITextFormattingCoordinator
```

## Topics

### Creating a Text-Formatting Coordinator

convenience init(for: UIWindowScene)

Creates a text-formatting coordinator for the specified window scene.

init(windowScene: UIWindowScene)

Initializes and returns a new text-formatting coordinator for the specified window scene.

### Showing the Font Panel

class var isFontPanelVisible: Bool

A Boolean value that indicates whether the font panel is visible.

class func toggleFontPanel(Any)

Toggles the visibility of the font panel.

### Configuring the Font Panel

func setSelectedAttributes([NSAttributedString.Key : Any], isMultiple: Bool)

Configures the initial display state of the font panel with the attributes of the selected text.

### Applying Updated Text Attributes

var delegate: (any UITextFormattingCoordinatorDelegate)?

The delegate of the text-formatting coordinator.

protocol UITextFormattingCoordinatorDelegate

The methods that delegates of text-formatting coordinators implement to apply font panel settings to the currently selected text.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIFontPickerViewControllerDelegate

## See Also

### Text formatting

typealias UITextAttributesConversionHandler

A handler for updating text with current font panel settings.

