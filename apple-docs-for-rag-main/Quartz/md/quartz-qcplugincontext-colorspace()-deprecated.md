

- Quartz
- QCPlugInContext
-  colorSpace() Deprecated

Instance Method

# colorSpace()

Returns the color space used by the rendering context.

macOS 10.4–10.15Deprecated

``` source
func colorSpace() -> Unmanaged!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

An RGB color space; `NULL` if the custom patch execution mode is not consumer.

## Discussion

If the method returns a color space, it must be an RGB color space.

## See Also

### Getting Execution Context Information

func userInfo() -> NSMutableDictionary!

Returns a mutable dictionary that contains information that can be shared between all instances of the `QCPlugIn` subclass, running in the same Quartz Composer context.

**Required**

Deprecated

func bounds() -> NSRect

Returns the bounds of the rendering context.

**Required**

Deprecated

