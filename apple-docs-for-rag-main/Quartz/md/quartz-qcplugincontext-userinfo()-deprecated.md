

- Quartz
- QCPlugInContext
-  userInfo() Deprecated

Instance Method

# userInfo()

Returns a mutable dictionary that contains information that can be shared between all instances of the `QCPlugIn` subclass, running in the same Quartz Composer context.

macOS 10.4–10.15Deprecated

``` source
func userInfo() -> NSMutableDictionary!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

A mutable dictionary.

## Discussion

When you add information to the dictionary, make sure that you use unique keys, such as `com.myCompany.foo`. You can use this dictionary to cache data that you want to share.

## See Also

### Getting Execution Context Information

func bounds() -> NSRect

Returns the bounds of the rendering context.

**Required**

Deprecated

func colorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space used by the rendering context.

**Required**

Deprecated

