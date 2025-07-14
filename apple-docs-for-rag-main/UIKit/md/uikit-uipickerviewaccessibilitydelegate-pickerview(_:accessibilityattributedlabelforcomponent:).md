

- UIKit
- UIPickerViewAccessibilityDelegate
-  pickerView(\_:accessibilityAttributedLabelForComponent:) 

Instance Method

# pickerView(\_:accessibilityAttributedLabelForComponent:)

Returns an attributed string that identifies the picker view component.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func pickerView(
    _ pickerView: UIPickerView,
    accessibilityAttributedLabelForComponent component: Int
) -> NSAttributedString?
```

## Parameters 

`pickerView`  

The picker view object.

`component`  

The component in the picker view that requires a label.

## Return Value

The attributed string that identifies the picker view component

## Discussion

Use this method to provide descriptive information for the components of a picker view. Your attributed string may include the accessibilitySpeechLanguage (Swift) or UIAccessibilitySpeechAttributeLanguage (Objective-C) attribute, which lets you use different language synthesizers for different parts of the string. The system prefers this method over the pickerView(_:accessibilityLabelForComponent:) method. For in-depth information on how to create an appropriate descriptive string, see Crafting Useful Labels and Hints.

## See Also

### Providing descriptive information

func pickerView(UIPickerView, accessibilityLabelForComponent: Int) -> String?

Returns a string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityHintForComponent: Int) -> String?

Returns a string that describes the result of performing an action on the component.

func pickerView(UIPickerView, accessibilityAttributedHintForComponent: Int) -> NSAttributedString?

Returns an attributed string that describes the result of performing an action on the specified component.

func pickerView(UIPickerView, accessibilityUserInputLabelsForComponent: Int) -> [String]

func pickerView(UIPickerView, accessibilityAttributedUserInputLabelsForComponent: Int) -> [NSAttributedString]

