

- Quartz
- QCPlugInOutputImageProvider
-  imageColorSpace() Deprecated

Instance Method

# imageColorSpace()

Returns the color space of the image or `NULL` if the image should not be color matched.

macOS 10.4–10.15Deprecated

``` source
func imageColorSpace() -> Unmanaged!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The color space of the image or `NULL`.

## See Also

### Providing Information About the Image

func imageBounds() -> NSRect

Returns the bounds of the image expressed in pixels and aligned to integer boundaries.

**Required**

Deprecated

func shouldColorMatch() -> Bool

Returns whether the image should be color matched.

Deprecated

