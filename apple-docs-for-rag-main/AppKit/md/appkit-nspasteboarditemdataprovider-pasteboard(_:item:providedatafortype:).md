

- AppKit
- NSPasteboardItemDataProvider
-  pasteboard(\_:item:provideDataForType:) 

Instance Method

# pasteboard(\_:item:provideDataForType:)

Asks the receiver to provide data for a specified type to a given pasteboard.

macOS 10.6+

``` source
nonisolated
func pasteboard(
    _ pasteboard: NSPasteboard?,
    item: NSPasteboardItem,
    provideDataForType type: NSPasteboard.PasteboardType
)
```

**Required**

## Parameters 

`pasteboard`  

A pasteboard to which the receiver has promised to provide data.

`item`  

A pasteboard item for which the receiver has promised to provide data

`type`  

A UTI type string.

## Discussion

The receiver was previously set as the provider using setDataProvider(_:forTypes:).

## See Also

### Related Documentation

Drag and Drop Programming Topics

Pasteboard Programming Guide

Services Implementation Guide

### Providing Data

func pasteboardFinishedWithDataProvider(NSPasteboard)

Informs the receiver that the pasteboard no longer needs the data provider for any of its pasteboard items.

