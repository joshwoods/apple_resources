

- XCUIAutomation
- XCUIElement
-  adjust(toNormalizedSliderPosition:) 

Instance Method

# adjust(toNormalizedSliderPosition:)

Manipulates the UI to change the value the slider displays to a new value, based on a normalized position.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func adjust(toNormalizedSliderPosition normalizedSliderPosition: CGFloat)
```

## Discussion

A normalized slider value of `0` corresponds to the minimum value of the slider, and `1` corresponds to the maximum value.

Note

The adjustment is a best effort to move the indicator to the desired position; absolute fidelity isn’t guaranteed.

## See Also

### Interacting with sliders

var normalizedSliderPosition: CGFloat

Returns the position of the slider’s indicator as a normalized value.

