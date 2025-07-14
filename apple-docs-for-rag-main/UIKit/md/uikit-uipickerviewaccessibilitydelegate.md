

- UIKit
-  UIPickerViewAccessibilityDelegate 

Protocol

# UIPickerViewAccessibilityDelegate

A set of methods you can implement to provide accessibility information for individual components of a picker view.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UIPickerViewAccessibilityDelegate : UIPickerViewDelegate
```

## Topics

### Providing descriptive information

func pickerView(UIPickerView, accessibilityLabelForComponent: Int) -> String?

Returns a string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityAttributedLabelForComponent: Int) -> NSAttributedString?

Returns an attributed string that identifies the picker view component.

func pickerView(UIPickerView, accessibilityHintForComponent: Int) -> String?

Returns a string that describes the result of performing an action on the component.

func pickerView(UIPickerView, accessibilityAttributedHintForComponent: Int) -> NSAttributedString?

Returns an attributed string that describes the result of performing an action on the specified component.

func pickerView(UIPickerView, accessibilityUserInputLabelsForComponent: Int) -> [String]

func pickerView(UIPickerView, accessibilityAttributedUserInputLabelsForComponent: Int) -> [NSAttributedString]

## Relationships

### Inherits From

- NSObjectProtocol
- UIPickerViewDelegate

## See Also

### Elements

class UIAccessibilityElement

An element that should be accessible to users with disabilities, but that isn’t accessible by default.

protocol UIScrollViewAccessibilityDelegate

A set of methods you can implement to provide accessibility information for a scroll view.

