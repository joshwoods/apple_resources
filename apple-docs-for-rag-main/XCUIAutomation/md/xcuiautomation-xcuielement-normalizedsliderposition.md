

- XCUIAutomation
- XCUIElement
-  normalizedSliderPosition 

Instance Property

# normalizedSliderPosition

Returns the position of the slider’s indicator as a normalized value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var normalizedSliderPosition: CGFloat { get }
```

## Discussion

A value of `0` corresponds to the minimum value of the slider, and `1` corresponds to its maximum value.

## See Also

### Interacting with sliders

func adjust(toNormalizedSliderPosition: CGFloat)

Manipulates the UI to change the value the slider displays to a new value, based on a normalized position.

