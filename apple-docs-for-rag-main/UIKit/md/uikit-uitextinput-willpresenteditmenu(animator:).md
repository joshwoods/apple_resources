

- UIKit
- UITextInput
-  willPresentEditMenu(animator:) 

Instance Method

# willPresentEditMenu(animator:)

Tells the object when the system is about to present an edit menu with an animator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func willPresentEditMenu(animator: any UIEditMenuInteractionAnimating)
```

## Parameters 

`animator`  

The appearance animator to add animations to, so that the animations will run alongside the appearance transition.

## See Also

### Managing the edit menu

func editMenu(for: UITextRange, suggestedActions: [UIMenuElement]) -> UIMenu?

Asks for the menu to display for the given text range and actions the system provides.

func willDismissEditMenu(animator: any UIEditMenuInteractionAnimating)

Tells the object when the system is about to dismiss an edit menu with an animator.

