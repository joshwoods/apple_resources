

- UIKit
- UITextFormattingCoordinator
-  delegate 

Instance Property

# delegate

The delegate of the text-formatting coordinator.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UITextFormattingCoordinatorDelegate)? { get set }
```

## See Also

### Applying Updated Text Attributes

protocol UITextFormattingCoordinatorDelegate

The methods that delegates of text-formatting coordinators implement to apply font panel settings to the currently selected text.

