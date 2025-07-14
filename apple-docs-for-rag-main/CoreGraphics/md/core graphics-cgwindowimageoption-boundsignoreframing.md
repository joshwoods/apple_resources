

- Core Graphics
- CGWindowImageOption
-  boundsIgnoreFraming 

Type Property

# boundsIgnoreFraming

Mac CatalystmacOS

``` source
static var boundsIgnoreFraming: CGWindowImageOption { get }
```

## Discussion

When the requested capture rectangle is CGRectNull, using this option captures the window area only and does not capture the area occupied by any window framing effects.

## See Also

### Type Properties

static var bestResolution: CGWindowImageOption

When capturing the window, return the best image resolution. The returned image size may be different than the screen size.

static var nominalResolution: CGWindowImageOption

When capturing the window, return the nominal image resolution. The returned image size is the same as the screen size.

static var onlyShadows: CGWindowImageOption

static var shouldBeOpaque: CGWindowImageOption

