

- UIKit
- UIPickerView
-  view(forRow:forComponent:) 

Instance Method

# view(forRow:forComponent:)

Returns the view used by the picker view for a given row and component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func view(
    forRow row: Int,
    forComponent component: Int
) -> UIView?
```

## Parameters 

`row`  

The zero-indexed number of a row of the picker view.

`component`  

The zero-indexed number of a component of the picker view.

## Return Value

The view provided by the delegate in the pickerView(_:viewForRow:forComponent:reusing:) method. Returns `nil` if the specified row of the component is not visible or if the delegate does not implement p`ickerView:viewForRow:forComponent:reusingView:`.

