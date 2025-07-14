

- UIKit
- UITextInput
-  editMenu(for:suggestedActions:) 

Instance Method

# editMenu(for:suggestedActions:)

Asks for the menu to display for the given text range and actions the system provides.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
optional func editMenu(
    for textRange: UITextRange,
    suggestedActions: [UIMenuElement]
) -> UIMenu?
```

## Parameters 

`textRange`  

The text range the menu is presenting for.

`suggestedActions`  

The actions and commands the system suggests.

## Return Value

Returns a menu describing the desired menu hierarchy. Return `nil` to present the default system menu.

## Discussion

The following example returns a menu with additional actions in a submenu.

```
func editMenu(for textRange: UITextRange, suggestedActions: [UIMenuElement]) -> UIMenu? {
    let indentationMenu = UIMenu(title: "Indentation", image: UIImage(systemName: "list.bullet.indent"), children: [
        UIAction(title: "Increase", image: UIImage(systemName: "increase.indent")) { (action) in
            // Increase indentation action.
        },
        UIAction(title: "Decrease", image: UIImage(systemName: "decrease.indent")) { (action) in
            // Decrease indentation action.
        }
    ])

    var actions = suggestedActions
    actions.append(indentationMenu)
    return UIMenu(children: actions)
}
```

## See Also

### Managing the edit menu

func willPresentEditMenu(animator: any UIEditMenuInteractionAnimating)

Tells the object when the system is about to present an edit menu with an animator.

func willDismissEditMenu(animator: any UIEditMenuInteractionAnimating)

Tells the object when the system is about to dismiss an edit menu with an animator.

