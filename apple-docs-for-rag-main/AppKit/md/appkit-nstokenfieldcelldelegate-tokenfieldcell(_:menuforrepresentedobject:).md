

- AppKit
- NSTokenFieldCellDelegate
-  tokenFieldCell(\_:menuForRepresentedObject:) 

Instance Method

# tokenFieldCell(\_:menuForRepresentedObject:)

Allows the delegate to provide a menu for the specified represented object.

macOS

``` source
@MainActor
optional func tokenFieldCell(
    _ tokenFieldCell: NSTokenFieldCell,
    menuForRepresentedObject representedObject: Any
) -> NSMenu?
```

## Parameters 

`tokenFieldCell`  

The token field cell that sent the message.

`representedObject`  

A represented object of the token field.

## Return Value

The menu associated with the represented object.

## Discussion

The returned menu should be autoreleased. By default tokens in a token field cell do not return menus.

## See Also

### Managing Menus for Represented Objects

func tokenFieldCell(NSTokenFieldCell, hasMenuForRepresentedObject: Any) -> Bool

Allows the delegate to specify whether the represented object provides a menu.

