

- UIKit
- UIMenuBuilder
-  replaceChildren(ofMenu:from:) 

Instance Method

# replaceChildren(ofMenu:from:)

Replaces the elements in a menu with the elements returned by the specified handler block.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func replaceChildren(
    ofMenu parentIdentifier: UIMenu.Identifier,
    from childrenBlock: ([UIMenuElement]) -> [UIMenuElement]
)
```

**Required**

## Parameters 

`parentIdentifier`  

The identifier of the menu containing the children to replace.

`childrenBlock`  

A handler that returns the menu elements that replace the children in the menu associated with `parentIdentifier`. This handler has the following parameter:

`oldChildren`  
The array of menu elements to replace.

## Discussion

Use this method to add, remove, and rearrange the children elements of a menu. For example, the following code listing uses this method to insert a Copy HTML menu element before Paste in the standardEdit menu.

```
builder.replaceChildren(ofMenu: .standardEdit) { (oldChildren) -> [UIMenuElement] in
    // Find the index of Paste menu element.
    var indexOfPaste = 0
    for (index, menuElement) in oldChildren.enumerated() {
        if let keyCommand = menuElement as? UIKeyCommand {
            if keyCommand.action == #selector(UIResponderStandardEditActions.paste(_:)) {
                indexOfPaste = index
                break
            }
        }
    }

    // Create a Copy HTML menu element.
    let copyHTML = UIKeyCommand(title: "Copy as HTML",
                                action: #selector(copyHTML(_:)),
                                input: "c",
                                modifierFlags: [.control, .command])

    // Insert Copy HTML before the Paste menu element
    // if found; otherwise, insert Copy HTML at the
    // beginning of the array.
    var newChildren = oldChildren
    newChildren.insert(copyHTML, at: indexOfPaste)
    return newChildren
}
```

## See Also

### Replacing menus and child menu elements

func replace(menu: UIMenu.Identifier, with: UIMenu)

Replaces the specified menu with a new menu.

**Required**

