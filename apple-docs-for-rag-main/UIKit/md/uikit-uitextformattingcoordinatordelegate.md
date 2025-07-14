

- UIKit
-  UITextFormattingCoordinatorDelegate 

Protocol

# UITextFormattingCoordinatorDelegate

The methods that delegates of text-formatting coordinators implement to apply font panel settings to the currently selected text.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
protocol UITextFormattingCoordinatorDelegate : NSObjectProtocol
```

## Topics

### Updating Text Attributes

func updateTextAttributes(conversionHandler: ([NSAttributedString.Key : Any]) -> [NSAttributedString.Key : Any])

Applies the current font panel settings to the selected text.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Applying Updated Text Attributes

var delegate: (any UITextFormattingCoordinatorDelegate)?

The delegate of the text-formatting coordinator.

