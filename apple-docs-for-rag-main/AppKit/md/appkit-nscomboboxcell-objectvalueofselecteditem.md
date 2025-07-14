

- AppKit
- NSComboBoxCell
-  objectValueOfSelectedItem 

Instance Property

# objectValueOfSelectedItem

The object corresponding to the last item selected from the pop-up list.

macOS

``` source
@MainActor
var objectValueOfSelectedItem: Any? { get }
```

## Discussion

The value of this property is the object from the combo box’s internal item list corresponding to the last item selected from the pop-up list, or `nil` if no item is selected.

Note that nothing is initially selected in a newly initialized combo box cell. Accessing this property logs a warning if usesDataSource is true.

## See Also

### Manipulating the Selection

func deselectItem(at: Int)

Deselects the pop-up list item at the given index if it’s selected.

var indexOfSelectedItem: Int

The index of the last item selected from the pop-up list.

func selectItem(at: Int)

Selects the pop-up list row at the given index.

func selectItem(withObjectValue: Any?)

Selects the first pop-up list item that corresponds to the specified object.

