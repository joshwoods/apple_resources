

- XCUIAutomation
- XCUIElement
-  adjust(toPickerWheelValue:) 

Instance Method

# adjust(toPickerWheelValue:)

Changes the value that the picker wheel displays.

iOSiPadOSMac CatalystXcode 16.3+

``` source
@MainActor
func adjust(toPickerWheelValue pickerWheelValue: String)
```

## Discussion

This method generates a test failure if the specified value isn’t available.

