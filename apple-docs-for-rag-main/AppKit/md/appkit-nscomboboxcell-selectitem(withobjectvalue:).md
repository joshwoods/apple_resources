

- AppKit
- NSComboBoxCell
-  selectItem(withObjectValue:) 

Instance Method

# selectItem(withObjectValue:)

Selects the first pop-up list item that corresponds to the specified object.

macOS

``` source
@MainActor
func selectItem(withObjectValue object: Any?)
```

## Parameters 

`object`  

The object for which to select the corresponding pop-up list item. Objects are considered equal if they have the same id or if `isEqual:` returns true.

## Discussion

This method logs a warning if usesDataSource is true. Posts an selectionDidChangeNotification to the default notification center if the selection does in fact change. Note that this method doesn’t alter the contents of the combo box cell’s text field—see Setting the Combo Box’s Value for more information.

## See Also

### Related Documentation

var objectValue: Any?

The value of the receiver’s cell as an Objective-C object.

### Manipulating the Selection

func deselectItem(at: Int)

Deselects the pop-up list item at the given index if it’s selected.

var indexOfSelectedItem: Int

The index of the last item selected from the pop-up list.

var objectValueOfSelectedItem: Any?

The object corresponding to the last item selected from the pop-up list.

func selectItem(at: Int)

Selects the pop-up list row at the given index.

