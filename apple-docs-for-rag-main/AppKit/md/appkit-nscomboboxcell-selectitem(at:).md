

- AppKit
- NSComboBoxCell
-  selectItem(at:) 

Instance Method

# selectItem(at:)

Selects the pop-up list row at the given index.

macOS

``` source
@MainActor
func selectItem(at index: Int)
```

## Parameters 

`index`  

The index of the row to select.

## Discussion

Posts an selectionDidChangeNotification to the default notification center if the selection does in fact change. Note that this method does not alter the contents of the combo box cell’s text field—see Combo Box Programming Topics for more information.

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

func selectItem(withObjectValue: Any?)

Selects the first pop-up list item that corresponds to the specified object.

