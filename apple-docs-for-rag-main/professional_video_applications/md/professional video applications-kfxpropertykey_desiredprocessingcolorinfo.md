

- Professional Video Applications
-  kFxPropertyKey_DesiredProcessingColorInfo 

Global Variable

# kFxPropertyKey_DesiredProcessingColorInfo

A key that determines whether your plug-in renders in linear or gamma-corrected color space.

FxPlug 3.1+

``` source
var kFxPropertyKey_DesiredProcessingColorInfo: String { get }
```

## Mentioned in 

Managing color space and gamut in plug-ins

## Discussion

The value for this key is an `NSUInteger` indicating the color space that the plug-in will process in. This color space is expressed as an FxImageColorInfo constant. If a plug-in includes this property, all inputs are in the specified color space, and the output must also be in this color space.

## See Also

### Property Keys

var kFxPropertyKey_NeedsFullBuffer: String

A key that determines whether the plug-in needs the entire image to do its processing, and can’t tile its rendering.

var kFxPropertyKey_VariesWhenParamsAreStatic: String

A key that determines whether your rendering varies even when the parameters remain the same.

var kFxPropertyKey_ChangesOutputSize: String

A key that determines whether your filter has the ability to change the size of its output to be different than the size of its input.

