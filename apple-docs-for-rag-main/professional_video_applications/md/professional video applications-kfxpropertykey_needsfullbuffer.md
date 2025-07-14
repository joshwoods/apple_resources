

- Professional Video Applications
-  kFxPropertyKey_NeedsFullBuffer 

Global Variable

# kFxPropertyKey_NeedsFullBuffer

A key that determines whether the plug-in needs the entire image to do its processing, and can’t tile its rendering.

FxPlug 4.0+

``` source
var kFxPropertyKey_NeedsFullBuffer: String { get }
```

## Mentioned in 

Building an FxPlug plug-in manually

Working with tiled images

## Discussion

This value of this key is a Boolean `NSNumber` indicating whether this plug-in needs the entire image to do its processing. Note that setting this value to `YES` incurs a significant performance penalty and makes your plug-in unable to render large input images. The default value is `NO`.

## See Also

### Property Keys

var kFxPropertyKey_VariesWhenParamsAreStatic: String

A key that determines whether your rendering varies even when the parameters remain the same.

var kFxPropertyKey_ChangesOutputSize: String

A key that determines whether your filter has the ability to change the size of its output to be different than the size of its input.

var kFxPropertyKey_DesiredProcessingColorInfo: String

A key that determines whether your plug-in renders in linear or gamma-corrected color space.

