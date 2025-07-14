

- Professional Video Applications
-  kFxPropertyKey_ChangesOutputSize 

Global Variable

# kFxPropertyKey_ChangesOutputSize

A key that determines whether your filter has the ability to change the size of its output to be different than the size of its input.

FxPlug 4.0+

``` source
var kFxPropertyKey_ChangesOutputSize: String { get }
```

## Discussion

The value of this key is a Boolean `NSNumber` that indicates whether your filter returns an output that has a different size than the input. If not, return `NO` and your filter’s destinationImageRect(_:sourceImages:destinationImage:pluginState:at:) method will not be called.

## See Also

### Property Keys

var kFxPropertyKey_NeedsFullBuffer: String

A key that determines whether the plug-in needs the entire image to do its processing, and can’t tile its rendering.

var kFxPropertyKey_VariesWhenParamsAreStatic: String

A key that determines whether your rendering varies even when the parameters remain the same.

var kFxPropertyKey_DesiredProcessingColorInfo: String

A key that determines whether your plug-in renders in linear or gamma-corrected color space.

