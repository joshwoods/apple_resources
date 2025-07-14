

- Core Graphics
- CGWindowImageOption
-  shouldBeOpaque 

Type Property

# shouldBeOpaque

Mac CatalystmacOS

``` source
static var shouldBeOpaque: CGWindowImageOption { get }
```

## Discussion

When capturing the window, partially transparent areas are backed by a solid white color so that the resulting image is fully opaque. You can combine this option with other options.

## See Also

### Type Properties

static var bestResolution: CGWindowImageOption

When capturing the window, return the best image resolution. The returned image size may be different than the screen size.

static var boundsIgnoreFraming: CGWindowImageOption

static var nominalResolution: CGWindowImageOption

When capturing the window, return the nominal image resolution. The returned image size is the same as the screen size.

static var onlyShadows: CGWindowImageOption

