

- Core Graphics
- CGWindowImageOption
-  bestResolution 

Type Property

# bestResolution

When capturing the window, return the best image resolution. The returned image size may be different than the screen size.

Mac CatalystmacOS

``` source
static var bestResolution: CGWindowImageOption { get }
```

## See Also

### Type Properties

static var boundsIgnoreFraming: CGWindowImageOption

static var nominalResolution: CGWindowImageOption

When capturing the window, return the nominal image resolution. The returned image size is the same as the screen size.

static var onlyShadows: CGWindowImageOption

static var shouldBeOpaque: CGWindowImageOption

