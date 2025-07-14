

- UIKit
- UIPickerViewAccessibilityDelegate
-  pickerView(\_:accessibilityHintForComponent:) 

Instance Method

# pickerView(\_:accessibilityHintForComponent:)

Returns a string that describes the result of performing an action on the component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    accessibilityHintForComponent component: Int
) -> String?
```

## Parameters 

`pickerView`  

The picker view object.

`component`  

The component in the picker view that requires a hint.

## Return Value

The localized string that describes the results of performing an action on the specified component.

## Discussion

Implement this optional method to ensure that the accessibility element representing the picker view provides an appropriate hint for each component. The system prefers the pickerView(_:accessibilityAttributedHintForComponent:) method over this one. For in-depth information on how to create an appropriate hint, see Guidelines for Creating Hints.

## See Also

### Providing descriptive information

func pickerView(UIPickerView, accessibilityLabelForComponent: Int) -> String?

Returns a string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityAttributedLabelForComponent: Int) -> NSAttributedString?

Returns an attributed string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityAttributedHintForComponent: Int) -> NSAttributedString?

Returns an attributed string that describes the result of performing an action on the specified component.

func pickerView(UIPickerView, accessibilityUserInputLabelsForComponent: Int) -> [String]

func pickerView(UIPickerView, accessibilityAttributedUserInputLabelsForComponent: Int) -> [NSAttributedString]

