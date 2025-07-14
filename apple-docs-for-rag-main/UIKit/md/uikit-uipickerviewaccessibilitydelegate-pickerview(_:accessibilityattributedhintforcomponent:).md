

- UIKit
- UIPickerViewAccessibilityDelegate
-  pickerView(\_:accessibilityAttributedHintForComponent:) 

Instance Method

# pickerView(\_:accessibilityAttributedHintForComponent:)

Returns an attributed string that describes the result of performing an action on the specified component.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    accessibilityAttributedHintForComponent component: Int
) -> NSAttributedString?
```

## Parameters 

`pickerView`  

The picker view object.

`component`  

The component in the picker view that requires a hint.

## Return Value

The localized attributed string that describes the results of performing an action on the specified component.

## Discussion

Implement this optional method to ensure that the accessibility element representing the picker view provides an appropriate hint for each component. Your attributed string may include the accessibilitySpeechLanguage (Swift) or UIAccessibilitySpeechAttributeLanguage (Objective-C) attribute, which lets you use different language synthesizers for different parts of the string. The system prefers this method over the pickerView(_:accessibilityHintForComponent:) method.

For in-depth information on how to create an appropriate hint, see Guidelines for Creating Hints.

## See Also

### Providing descriptive information

func pickerView(UIPickerView, accessibilityLabelForComponent: Int) -> String?

Returns a string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityAttributedLabelForComponent: Int) -> NSAttributedString?

Returns an attributed string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityHintForComponent: Int) -> String?

Returns a string that describes the result of performing an action on the component.

func pickerView(UIPickerView, accessibilityUserInputLabelsForComponent: Int) -> [String]

func pickerView(UIPickerView, accessibilityAttributedUserInputLabelsForComponent: Int) -> [NSAttributedString]

