

- UIKit
- UIPickerView
-  rowSize(forComponent:) 

Instance Method

# rowSize(forComponent:)

Returns the size of a row for a component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func rowSize(forComponent component: Int) -> CGSize
```

## Parameters 

`component`  

A zero-indexed number identifying a component.

## Return Value

The size of rows in the given component. This is generally the size required to display the largest string or view used as a row in the component.

## Discussion

A picker view fetches the value of this property by calling the pickerView(_:widthForComponent:) and pickerView(_:rowHeightForComponent:) delegate methods, and caches it. The default value is (`0`, `0`).

## See Also

### Getting the dimensions of the picker view

var numberOfComponents: Int

The number of components for the picker view.

func numberOfRows(inComponent: Int) -> Int

Returns the number of rows for a component.

