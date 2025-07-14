

- AppKit
- NSComboBox
-  deselectItem(at:) 

Instance Method

# deselectItem(at:)

Deselects the pop-up list item at the specified index if it’s selected.

macOS

``` source
@MainActor
func deselectItem(at index: Int)
```

## Parameters 

`index`  

The index of the item to deselect.

## Discussion

If the selection does in fact change, this method posts an selectionDidChangeNotification to the default notification center.

## See Also

### Related Documentation

var numberOfItems: Int

The total number of items in the pop-up list.

### Manipulating the Selection

var indexOfSelectedItem: Int

The index of the last item selected from the pop-up list.

var objectValueOfSelectedItem: Any?

The object corresponding to the last item selected from the pop-up list.

func selectItem(at: Int)

Selects the pop-up list row at the given index.

func selectItem(withObjectValue: Any?)

Selects the first pop-up list item that corresponds to the given object.

