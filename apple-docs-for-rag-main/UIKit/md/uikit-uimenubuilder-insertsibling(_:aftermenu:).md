

- UIKit
- UIMenuBuilder
-  insertSibling(\_:afterMenu:) 

Instance Method

# insertSibling(\_:afterMenu:)

Inserts a sibling menu after the specified menu.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func insertSibling(
    _ siblingMenu: UIMenu,
    afterMenu siblingIdentifier: UIMenu.Identifier
)
```

**Required**

## Parameters 

`siblingMenu`  

The sibling menu to insert.

`siblingIdentifier`  

The identifier of the menu that comes before the inserted sibling menu.

## See Also

### Inserting sibling menus

func insertSibling(UIMenu, beforeMenu: UIMenu.Identifier)

Inserts a sibling menu before the specified menu.

**Required**

