

- UIKit
- UIPickerViewDelegate
-  pickerView(\_:titleForRow:forComponent:) 

Instance Method

# pickerView(\_:titleForRow:forComponent:)

Called by the picker view when it needs the title to use for a given row in a given component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    titleForRow row: Int,
    forComponent component: Int
) -> String?
```

## Parameters 

`pickerView`  

An object representing the picker view requesting the data.

`row`  

A zero-indexed number identifying a row of `component`. Rows are numbered top-to-bottom.

`component`  

A zero-indexed number identifying a component of `pickerView`. Components are numbered left-to-right.

## Return Value

The string to use as the title of the indicated component row.

## Discussion

If you implement both this method and the pickerView(_:attributedTitleForRow:forComponent:) method, the picker view prefers the pickerView(_:attributedTitleForRow:forComponent:) method. However, if that method returns `nil`, the picker view falls back to using the string returned by this method.

## See Also

### Setting the content of component rows

func pickerView(UIPickerView, attributedTitleForRow: Int, forComponent: Int) -> NSAttributedString?

Called by the picker view when it needs the styled title to use for a given row in a given component.

func pickerView(UIPickerView, viewForRow: Int, forComponent: Int, reusing: UIView?) -> UIView

Called by the picker view when it needs the view to use for a given row in a given component.

