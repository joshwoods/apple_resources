

- Quartz
- QCPlugInOutputImageProvider
-  shouldColorMatch() Deprecated

Instance Method

# shouldColorMatch()

Returns whether the image should be color matched.

macOS 10.4–10.15Deprecated

``` source
optional func shouldColorMatch() -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

false if the image is a mask or gradient; otherwise true, which is the default.

## See Also

### Providing Information About the Image

func imageBounds() -> NSRect

Returns the bounds of the image expressed in pixels and aligned to integer boundaries.

**Required**

Deprecated

func imageColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the image or `NULL` if the image should not be color matched.

**Required**

Deprecated

