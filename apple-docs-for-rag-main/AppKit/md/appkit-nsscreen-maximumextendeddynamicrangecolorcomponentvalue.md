

- AppKit
- NSScreen
-  maximumExtendedDynamicRangeColorComponentValue 

Instance Property

# maximumExtendedDynamicRangeColorComponentValue

The current maximum color component value for the screen.

macOS 10.11+

``` source
var maximumExtendedDynamicRangeColorComponentValue: CGFloat { get }
```

## Discussion

If no content on screen provides extended dynamic range (EDR) values, the value of this property is `1.0`. If any content onscreen has requested EDR, the value may be greater than `1.0`, depending on the capabilities of the display hardware and other conditions. Only rendering contexts that support EDR can use values greater than `1.0`.

When the value changes, didChangeScreenParametersNotification is posted.

## See Also

### Related Documentation

var wantsExtendedDynamicRangeContent: Bool { get set }

Enables extended dynamic range values onscreen.

### Getting Extended Dynamic Range Details

var maximumPotentialExtendedDynamicRangeColorComponentValue: CGFloat

The maximum possible color component value for the screen when it’s in extended dynamic range (EDR) mode.

var maximumReferenceExtendedDynamicRangeColorComponentValue: CGFloat

The current maximum color component value for reference rendering to the screen.

