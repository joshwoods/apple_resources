

- UIKit
- UIPickerViewDelegate
-  pickerView(\_:attributedTitleForRow:forComponent:) 

Instance Method

# pickerView(\_:attributedTitleForRow:forComponent:)

Called by the picker view when it needs the styled title to use for a given row in a given component.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    attributedTitleForRow row: Int,
    forComponent component: Int
) -> NSAttributedString?
```

## Parameters 

`pickerView`  

An object representing the picker view requesting the data.

`row`  

A zero-indexed number identifying a row of `component`. Rows are numbered top-to-bottom.

`component`  

A zero-indexed number identifying a component of `pickerView`. Components are numbered left-to-right.

## Return Value

The attributed string to use as the title of the indicated component row.

## Discussion

If you implement both this method and the pickerView(_:titleForRow:forComponent:) method, the picker view prefers the use of this method. However, if your implementation of this method returns `nil`, the picker view falls back to using the string returned by the pickerView(_:titleForRow:forComponent:) method.

## See Also

### Setting the content of component rows

func pickerView(UIPickerView, titleForRow: Int, forComponent: Int) -> String?

Called by the picker view when it needs the title to use for a given row in a given component.

func pickerView(UIPickerView, viewForRow: Int, forComponent: Int, reusing: UIView?) -> UIView

Called by the picker view when it needs the view to use for a given row in a given component.

