

- UIKit
- UIPickerViewDelegate
-  pickerView(\_:didSelectRow:inComponent:) 

Instance Method

# pickerView(\_:didSelectRow:inComponent:)

Called by the picker view when the user selects a row in a component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    didSelectRow row: Int,
    inComponent component: Int
)
```

## Parameters 

`pickerView`  

An object representing the picker view requesting the data.

`row`  

A zero-indexed number identifying a row of `component`. Rows are numbered top-to-bottom.

`component`  

A zero-indexed number identifying a component of `pickerView`. Components are numbered left-to-right.

## Discussion

To determine what value the user selected, the delegate uses the `row` index to access the value at the corresponding position in the array used to construct the component.

