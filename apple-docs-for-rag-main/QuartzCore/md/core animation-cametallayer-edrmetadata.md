

- Core Animation
- CAMetalLayer
-  edrMetadata 

Instance Property

# edrMetadata

Metadata describing the tone mapping to apply to the extended dynamic range (EDR) values in the layer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.15+visionOS 1.0+

``` source
var edrMetadata: CAEDRMetadata? { get set }
```

## Discussion

You must set this property before calling nextDrawable().

The default value is `nil`, which means that the system doesn’t perform any tone mapping of data prior to passing it on to the display. Values above the maximum (maximumExtendedDynamicRangeColorComponentValue) may be clipped.

If non-`nil`, the system uses the metadata provided to tone map values to the display, based on the display’s current characteristics. You must also set pixelFormat to a pixel format that supports pixel values greater than `1.0` (such as MTLPixelFormat.rgba16Float) and colorspace to a color space that supports a linear transfer function.

The tone mapping process requires significant amounts of memory and GPU processing.

## See Also

### Configuring Extended Dynamic Range Behavior

var wantsExtendedDynamicRangeContent: Bool

Enables extended dynamic range values onscreen.

