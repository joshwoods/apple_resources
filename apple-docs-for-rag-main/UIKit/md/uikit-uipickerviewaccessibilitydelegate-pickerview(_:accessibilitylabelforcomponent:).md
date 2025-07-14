

- UIKit
- UIPickerViewAccessibilityDelegate
-  pickerView(\_:accessibilityLabelForComponent:) 

Instance Method

# pickerView(\_:accessibilityLabelForComponent:)

Returns a string that identifies the picker view component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    accessibilityLabelForComponent component: Int
) -> String?
```

## Parameters 

`pickerView`  

The picker view object.

`component`  

The component in the picker view that requires a label.

## Return Value

A succinct label, in a localized string, that identifies the picker view component.

## Discussion

Implement this optional method to ensure that the accessibility element representing the picker view provides an appropriate label for each component. The system prefers the pickerView(_:accessibilityAttributedLabelForComponent:) method over this one. For in-depth information on how to create an appropriate label, see Crafting Useful Labels and Hints.

## See Also

### Providing descriptive information

func pickerView(UIPickerView, accessibilityAttributedLabelForComponent: Int) -> NSAttributedString?

Returns an attributed string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityHintForComponent: Int) -> String?

Returns a string that describes the result of performing an action on the component.

func pickerView(UIPickerView, accessibilityAttributedHintForComponent: Int) -> NSAttributedString?

Returns an attributed string that describes the result of performing an action on the specified component.

func pickerView(UIPickerView, accessibilityUserInputLabelsForComponent: Int) -> [String]

func pickerView(UIPickerView, accessibilityAttributedUserInputLabelsForComponent: Int) -> [NSAttributedString]

