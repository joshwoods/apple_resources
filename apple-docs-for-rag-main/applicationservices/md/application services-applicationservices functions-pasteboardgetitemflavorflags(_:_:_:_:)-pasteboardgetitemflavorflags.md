

- Application Services
- ApplicationServices Functions
-  PasteboardGetItemFlavorFlags(\_:\_:\_:\_:) 

Function

# PasteboardGetItemFlavorFlags(\_:\_:\_:\_:)

macOS 10.3+

``` source
func PasteboardGetItemFlavorFlags(
    _ inPasteboard: Pasteboard,
    _ inItem: PasteboardItemID,
    _ inFlavorType: CFString,
    _ outFlags: UnsafeMutablePointer
) -> OSStatus
```

