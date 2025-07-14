

- Application Services
- ApplicationServices Functions
-  PasteboardPutItemFlavor(\_:\_:\_:\_:\_:) 

Function

# PasteboardPutItemFlavor(\_:\_:\_:\_:\_:)

macOS 10.3+

``` source
func PasteboardPutItemFlavor(
    _ inPasteboard: Pasteboard,
    _ inItem: PasteboardItemID,
    _ inFlavorType: CFString,
    _ inData: CFData?,
    _ inFlags: PasteboardFlavorFlags
) -> OSStatus
```

