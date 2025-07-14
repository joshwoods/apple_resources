

- Quartz
- QCPlugInInputImageSource
-  shouldColorMatch() Deprecated

Instance Method

# shouldColorMatch()

Returns whether or not the image source should be color matched.

macOS 10.4–10.15Deprecated

``` source
func shouldColorMatch() -> Bool
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

false if the source is a mask or gradient; true otherwise.

## See Also

### Getting Color Space Information

func imageColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the image source.

**Required**

Deprecated

