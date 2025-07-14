

- UIKit
- UIPickerViewAccessibilityDelegate
-  pickerView(\_:accessibilityUserInputLabelsForComponent:) 

Instance Method

# pickerView(\_:accessibilityUserInputLabelsForComponent:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    accessibilityUserInputLabelsForComponent component: Int
) -> [String]
```

## See Also

### Providing descriptive information

func pickerView(UIPickerView, accessibilityLabelForComponent: Int) -> String?

Returns a string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityAttributedLabelForComponent: Int) -> NSAttributedString?

Returns an attributed string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityHintForComponent: Int) -> String?

Returns a string that describes the result of performing an action on the component.

func pickerView(UIPickerView, accessibilityAttributedHintForComponent: Int) -> NSAttributedString?

Returns an attributed string that describes the result of performing an action on the specified component.

func pickerView(UIPickerView, accessibilityAttributedUserInputLabelsForComponent: Int) -> [NSAttributedString]

