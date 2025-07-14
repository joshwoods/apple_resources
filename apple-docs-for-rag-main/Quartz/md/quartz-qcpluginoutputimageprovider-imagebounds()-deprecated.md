

- Quartz
- QCPlugInOutputImageProvider
-  imageBounds() Deprecated

Instance Method

# imageBounds()

Returns the bounds of the image expressed in pixels and aligned to integer boundaries.

macOS 10.4–10.15Deprecated

``` source
func imageBounds() -> NSRect
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The bounds of the image. Note that the `QCPlugIn` class does not support images that have infinite bounds.

## See Also

### Providing Information About the Image

func imageColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the image or `NULL` if the image should not be color matched.

**Required**

Deprecated

func shouldColorMatch() -> Bool

Returns whether the image should be color matched.

Deprecated

