

- UIKit
- UIPickerView
-  selectedRow(inComponent:) 

Instance Method

# selectedRow(inComponent:)

Returns the index of the selected row in a given component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func selectedRow(inComponent component: Int) -> Int
```

## Parameters 

`component`  

A zero-indexed number identifying a component of the picker view.

## Return Value

A zero-indexed number identifying the selected row, or `-1` if no row is selected.

## See Also

### Selecting rows in the view picker

func selectRow(Int, inComponent: Int, animated: Bool)

Selects a row in a specified component of the picker view.

