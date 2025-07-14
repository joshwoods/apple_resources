

- UIKit
- UITextFieldDelegate
-  textField(\_:willDismissEditMenuWith:) 

Instance Method

# textField(\_:willDismissEditMenuWith:)

Tells the delegate that the system is about to dismiss an edit menu with an animator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func textField(
    _ textField: UITextField,
    willDismissEditMenuWith animator: any UIEditMenuInteractionAnimating
)
```

## Parameters 

`textField`  

The text field showing the menu.

`animator`  

The dismissal animator to add animations to, so that the animations will run alongside the dismissal transition.

## See Also

### Customizing an edit menu

func textField(UITextField, willPresentEditMenuWith: any UIEditMenuInteractionAnimating)

Tells the delegate that the system is about to present an edit menu with an animator.

