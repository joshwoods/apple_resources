

- AppKit
- NSSliderTouchBarItem
-  slider 

Instance Property

# slider

The slider displayed by the bar item.

macOS 10.12.2+

``` source
@MainActor
var slider: NSSlider { get set }
```

## Discussion

The slider is automatically created by the item, but you can provide a custom subclass to this property to customize behavior.

## See Also

### Configuring the slider

var label: String?

The text displayed alongside the slider.

var view: any NSView &amp; NSUserInterfaceCompression

