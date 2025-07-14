

- UIKit
- UIPickerViewDelegate
-  pickerView(\_:widthForComponent:) 

Instance Method

# pickerView(\_:widthForComponent:)

Called by the picker view when it needs the row width to use for drawing row content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    widthForComponent component: Int
) -> CGFloat
```

## Parameters 

`pickerView`  

The picker view requesting this information.

`component`  

A zero-indexed number identifying a component of the picker view. Components are numbered left-to-right.

## Return Value

A float value indicating the width of the row in points.

## See Also

### Setting the dimensions of the picker view

func pickerView(UIPickerView, rowHeightForComponent: Int) -> CGFloat

Called by the picker view when it needs the row height to use for drawing row content.

