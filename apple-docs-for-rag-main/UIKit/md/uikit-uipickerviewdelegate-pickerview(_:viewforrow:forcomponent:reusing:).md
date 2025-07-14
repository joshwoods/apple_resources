

- UIKit
- UIPickerViewDelegate
-  pickerView(\_:viewForRow:forComponent:reusing:) 

Instance Method

# pickerView(\_:viewForRow:forComponent:reusing:)

Called by the picker view when it needs the view to use for a given row in a given component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    viewForRow row: Int,
    forComponent component: Int,
    reusing view: UIView?
) -> UIView
```

## Parameters 

`pickerView`  

An object representing the picker view requesting the data.

`row`  

A zero-indexed number identifying a row of `component`. Rows are numbered top-to-bottom.

`component`  

A zero-indexed number identifying a component of `pickerView`. Components are numbered left-to-right.

`view`  

A view object that was previously used for this row, but is now hidden and cached by the picker view.

## Return Value

A view object to use as the content of `row`. The object can be any subclass of UIView, such as UILabel, UIImageView, or even a custom view.

## Discussion

If the previously used view (the `view` parameter) is adequate, return that. If you return a different view, the previously used view is released. The picker view centers the returned view in the rectangle for `row`.

## See Also

### Setting the content of component rows

func pickerView(UIPickerView, titleForRow: Int, forComponent: Int) -> String?

Called by the picker view when it needs the title to use for a given row in a given component.

func pickerView(UIPickerView, attributedTitleForRow: Int, forComponent: Int) -> NSAttributedString?

Called by the picker view when it needs the styled title to use for a given row in a given component.

