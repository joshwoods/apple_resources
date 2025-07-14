

- AppKit
- NSComboBoxCell
-  indexOfSelectedItem 

Instance Property

# indexOfSelectedItem

The index of the last item selected from the pop-up list.

macOS

``` source
@MainActor
var indexOfSelectedItem: Int { get }
```

## Discussion

The index of the last item selected from the combo box’s pop-up list or –1 if no item is selected. Note that nothing is initially selected in a newly initialized combo box cell.

## See Also

### Manipulating the Selection

func deselectItem(at: Int)

Deselects the pop-up list item at the given index if it’s selected.

var objectValueOfSelectedItem: Any?

The object corresponding to the last item selected from the pop-up list.

func selectItem(at: Int)

Selects the pop-up list row at the given index.

func selectItem(withObjectValue: Any?)

Selects the first pop-up list item that corresponds to the specified object.

