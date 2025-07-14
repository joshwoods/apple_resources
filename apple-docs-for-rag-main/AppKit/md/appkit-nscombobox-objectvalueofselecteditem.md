

- AppKit
- NSComboBox
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

For combo boxes that use their own internally maintained list of items, this property contains the object in that list that is selected. If no item is selected, the value in this property is `nil`. Nothing is selected in a newly initialized combo box. This method logs a warning if the usesDataSource property is true.

## See Also

### Manipulating the Selection

func deselectItem(at: Int)

Deselects the pop-up list item at the specified index if it’s selected.

var indexOfSelectedItem: Int

The index of the last item selected from the pop-up list.

func selectItem(at: Int)

Selects the pop-up list row at the given index.

func selectItem(withObjectValue: Any?)

Selects the first pop-up list item that corresponds to the given object.

