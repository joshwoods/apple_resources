

- AppKit
- NSPasteboardItemDataProvider
-  pasteboardFinishedWithDataProvider(\_:) 

Instance Method

# pasteboardFinishedWithDataProvider(\_:)

Informs the receiver that the pasteboard no longer needs the data provider for any of its pasteboard items.

macOS

``` source
nonisolated
optional func pasteboardFinishedWithDataProvider(_ pasteboard: NSPasteboard)
```

## Parameters 

`pasteboard`  

A pasteboard.

## Discussion

One data provider can provide data for more than one pasteboard item. This method is called when the pasteboard no longer needs the data provider for any of its pasteboard items. This can be either because the data provider has fulfilled all promises, or because ownership of the pasteboard has changed.

## See Also

### Providing Data

func pasteboard(NSPasteboard?, item: NSPasteboardItem, provideDataForType: NSPasteboard.PasteboardType)

Asks the receiver to provide data for a specified type to a given pasteboard.

**Required**

