

- AppKit
- NSTokenFieldCellDelegate
-  tokenFieldCell(\_:styleForRepresentedObject:) 

Instance Method

# tokenFieldCell(\_:styleForRepresentedObject:)

Allows the delegate to return the token style for editing the specified represented object.

macOS

``` source
@MainActor
optional func tokenFieldCell(
    _ tokenFieldCell: NSTokenFieldCell,
    styleForRepresentedObject representedObject: Any
) -> NSTokenField.TokenStyle
```

## Parameters 

`tokenFieldCell`  

The token field cell that sent the message.

`representedObject`  

A represented object of the token field cell.

## Return Value

The style that should be used to display the representedObject. Possible values are shown in NSTokenStyle_Values.

## Discussion

If the delegate implements this method and returns an NSTokenField.TokenStyle that differs from the style set by tokenStyle, the value the delegate returns is preferred.

If the delegate does not implement this method, the token field cell’s tokenStyle is used.

## See Also

### Displaying Tokenized Strings

func tokenFieldCell(NSTokenFieldCell, displayStringForRepresentedObject: Any) -> String?

Allows the delegate to provide a string to be displayed as a proxy for the represented object.

