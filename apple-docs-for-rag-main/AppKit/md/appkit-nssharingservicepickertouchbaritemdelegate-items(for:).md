

- AppKit
- NSSharingServicePickerTouchBarItemDelegate
-  items(for:) 

Instance Method

# items(for:)

Asks the delegate for items that represent the objects to be shared.

macOS 10.12.2+

``` source
@MainActor
func items(for pickerTouchBarItem: NSSharingServicePickerTouchBarItem) -> [Any]
```

**Required**

## Parameters 

`pickerTouchBarItem`  

The sharing service picker item that is requesting the items to be shared.

## Return Value

An array of items that represents the objects to be shared. Each element of the array must either conform to the NSPasteboardWriting protocol, or be an NSItemProvider.

