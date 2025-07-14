

- Quartz
- QCPlugInContext
-  bounds() Deprecated

Instance Method

# bounds()

Returns the bounds of the rendering context.

macOS 10.4–10.15Deprecated

``` source
func bounds() -> NSRect
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The bounds of the rendering context expressed in Quartz Composer units.

## See Also

### Getting Execution Context Information

func userInfo() -> NSMutableDictionary!

Returns a mutable dictionary that contains information that can be shared between all instances of the `QCPlugIn` subclass, running in the same Quartz Composer context.

**Required**

Deprecated

func colorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space used by the rendering context.

**Required**

Deprecated

