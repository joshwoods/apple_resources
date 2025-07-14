

- UIKit
- UIMenuBuilder
-  insertChild(\_:atStartOfMenu:) 

Instance Method

# insertChild(\_:atStartOfMenu:)

Adds a child menu as the first element of the specified parent menu.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func insertChild(
    _ childMenu: UIMenu,
    atStartOfMenu parentIdentifier: UIMenu.Identifier
)
```

**Required**

## Parameters 

`childMenu`  

The child menu to insert.

`parentIdentifier`  

The identifier of the parent menu in which to insert the child menu.

## See Also

### Inserting child menus

func insertChild(UIMenu, atEndOfMenu: UIMenu.Identifier)

Adds a child menu as the last element of the specified parent menu.

**Required**

