

- AppKit
- NSTokenFieldCellDelegate
-  tokenFieldCell(\_:hasMenuForRepresentedObject:) 

Instance Method

# tokenFieldCell(\_:hasMenuForRepresentedObject:)

Allows the delegate to specify whether the represented object provides a menu.

macOS

``` source
@MainActor
optional func tokenFieldCell(
    _ tokenFieldCell: NSTokenFieldCell,
    hasMenuForRepresentedObject representedObject: Any
) -> Bool
```

## Parameters 

`tokenFieldCell`  

The token field cell that sent the message.

`representedObject`  

A represented object of the token field.

## Return Value

true if the represented object has a menu, false otherwise.

## Discussion

By default tokens have no menus.

## See Also

### Managing Menus for Represented Objects

func tokenFieldCell(NSTokenFieldCell, menuForRepresentedObject: Any) -> NSMenu?

Allows the delegate to provide a menu for the specified represented object.

