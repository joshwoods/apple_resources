

- AppKit
- NSTokenFieldCellDelegate
-  tokenFieldCell(\_:displayStringForRepresentedObject:) 

Instance Method

# tokenFieldCell(\_:displayStringForRepresentedObject:)

Allows the delegate to provide a string to be displayed as a proxy for the represented object.

macOS

``` source
@MainActor
optional func tokenFieldCell(
    _ tokenFieldCell: NSTokenFieldCell,
    displayStringForRepresentedObject representedObject: Any
) -> String?
```

## Parameters 

`tokenFieldCell`  

The token field cell that sent the message.

`representedObject`  

A represented object of the token field cell.

## Return Value

The string to be used as a proxy for `representedObject`. If you return `nil` or do not implement this method, then `representedObject` is displayed as the string.

## See Also

### Related Documentation

Token Field Programming Guide

### Displaying Tokenized Strings

func tokenFieldCell(NSTokenFieldCell, styleForRepresentedObject: Any) -> NSTokenField.TokenStyle

Allows the delegate to return the token style for editing the specified represented object.

