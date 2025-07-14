

- Core Animation
- CAMetalLayer
-  wantsExtendedDynamicRangeContent 

Instance Property

# wantsExtendedDynamicRangeContent

Enables extended dynamic range values onscreen.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.11+visionOS 1.0+

``` source
var wantsExtendedDynamicRangeContent: Bool { get set }
```

## Discussion

The default value is false. If any onscreen layer has this property set to true, all rendered content is clamped to the screen’s maximumExtendedDynamicRangeColorComponentValue value rather than `1.0`.

## See Also

### Related Documentation

var maximumExtendedDynamicRangeColorComponentValue: CGFloat { get }

The current maximum color component value for the screen.

### Configuring Extended Dynamic Range Behavior

var edrMetadata: CAEDRMetadata?

Metadata describing the tone mapping to apply to the extended dynamic range (EDR) values in the layer.

