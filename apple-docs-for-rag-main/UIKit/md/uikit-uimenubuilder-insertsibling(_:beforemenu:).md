

- UIKit
- UIMenuBuilder
-  insertSibling(\_:beforeMenu:) 

Instance Method

# insertSibling(\_:beforeMenu:)

Inserts a sibling menu before the specified menu.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func insertSibling(
    _ siblingMenu: UIMenu,
    beforeMenu siblingIdentifier: UIMenu.Identifier
)
```

**Required**

## Parameters 

`siblingMenu`  

The sibling menu to insert.

`siblingIdentifier`  

The identifier of the menu that comes after the inserted sibling menu.

## See Also

### Inserting sibling menus

func insertSibling(UIMenu, afterMenu: UIMenu.Identifier)

Inserts a sibling menu after the specified menu.

**Required**

