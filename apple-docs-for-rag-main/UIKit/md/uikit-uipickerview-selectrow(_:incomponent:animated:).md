

- UIKit
- UIPickerView
-  selectRow(\_:inComponent:animated:) 

Instance Method

# selectRow(\_:inComponent:animated:)

Selects a row in a specified component of the picker view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func selectRow(
    _ row: Int,
    inComponent component: Int,
    animated: Bool
)
```

## Parameters 

`row`  

A zero-indexed number identifying a row of `component`.

`component`  

A zero-indexed number identifying a component of the picker view.

`animated`  

true to animate the selection by spinning the wheel (component) to the new value; if you specify false, the new selection is shown immediately.

## See Also

### Selecting rows in the view picker

func selectedRow(inComponent: Int) -> Int

Returns the index of the selected row in a given component.

