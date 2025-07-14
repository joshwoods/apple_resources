

- UIKit
- UIMenuBuilder
-  remove(menu:) 

Instance Method

# remove(menu:)

Removes a menu from the menu system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func remove(menu removedIdentifier: UIMenu.Identifier)
```

**Required**

## Parameters 

`removedIdentifier`  

The identifier of the menu element to remove.

## Discussion

Use this method to remove menus (UIMenu objects) from a menu system.

