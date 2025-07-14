

- Application Services
- ApplicationServices Functions
-  PasteboardCopyItemFlavorData(\_:\_:\_:\_:) 

Function

# PasteboardCopyItemFlavorData(\_:\_:\_:\_:)

macOS 10.3+

``` source
func PasteboardCopyItemFlavorData(
    _ inPasteboard: Pasteboard,
    _ inItem: PasteboardItemID,
    _ inFlavorType: CFString,
    _ outData: UnsafeMutablePointer
) -> OSStatus
```

