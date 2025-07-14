

- AppKit
- NSSliderTouchBarItem
-  valueAccessoryWidth 

Instance Property

# valueAccessoryWidth

The width of the value accessories that appear at either end of the slider.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var valueAccessoryWidth: NSSliderAccessory.Width { get set }
```

## Discussion

You can provide your own custom width, or use the system-provided default or wide options.

The default value is default.

## See Also

### Configuring slider accessories

var minimumValueAccessory: NSSliderAccessory?

The accessory that appears at the end of the slider with the minimum value.

var maximumValueAccessory: NSSliderAccessory?

The accessory that appears at the end of the slider with the maximum value.

