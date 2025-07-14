

- UIKit
- UIMenuBuilder
-  replace(menu:with:) 

Instance Method

# replace(menu:with:)

Replaces the specified menu with a new menu.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func replace(
    menu replacedIdentifier: UIMenu.Identifier,
    with replacementMenu: UIMenu
)
```

**Required**

## Parameters 

`replacedIdentifier`  

The identifier of the menu to replace.

`replacementMenu`  

The replacement menu.

## See Also

### Replacing menus and child menu elements

func replaceChildren(ofMenu: UIMenu.Identifier, from: ([UIMenuElement]) -> [UIMenuElement])

Replaces the elements in a menu with the elements returned by the specified handler block.

**Required**

