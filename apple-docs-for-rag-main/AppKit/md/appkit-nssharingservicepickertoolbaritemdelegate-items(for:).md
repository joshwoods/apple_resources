

- AppKit
- NSSharingServicePickerToolbarItemDelegate
-  items(for:) 

Instance Method

# items(for:)

Asks the delegate for the items to share.

macOS 10.15+

``` source
@MainActor
func items(for pickerToolbarItem: NSSharingServicePickerToolbarItem) -> [Any]
```

**Required**

## Parameters 

`pickerToolbarItem`  

The toolbar item that displays the share sheet.

## Return Value

An array of items to share using the share sheet.

## Discussion

In your implementation of this method, return the items in the current window that you want to share. Return the content that is focal to your window or is currently selected. For example, you might share the current photo someone is viewing. For a document window, you might share the document itself.

