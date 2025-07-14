

- Professional Video Applications
-  kFxPropertyKey_VariesWhenParamsAreStatic 

Global Variable

# kFxPropertyKey_VariesWhenParamsAreStatic

A key that determines whether your rendering varies even when the parameters remain the same.

FxPlug 4.0+

``` source
var kFxPropertyKey_VariesWhenParamsAreStatic: String { get }
```

## Mentioned in 

Building an FxPlug plug-in manually

## Discussion

The value for this key is a Boolean `NSNumber` indicating whether this effect changes its rendering even when the parameters don’t change. This can happen if your rendering is based on timing in addition to parameters, for example. Note that this property is only checked once when the filter is applied, so it should go in static properties rather than dynamic properties.

## See Also

### Property Keys

var kFxPropertyKey_NeedsFullBuffer: String

A key that determines whether the plug-in needs the entire image to do its processing, and can’t tile its rendering.

var kFxPropertyKey_ChangesOutputSize: String

A key that determines whether your filter has the ability to change the size of its output to be different than the size of its input.

var kFxPropertyKey_DesiredProcessingColorInfo: String

A key that determines whether your plug-in renders in linear or gamma-corrected color space.

