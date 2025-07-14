

- Core Graphics
- CGWindowListOption
-  optionAll 

Type Property

# optionAll

Mac CatalystmacOS

``` source
static var optionAll: CGWindowListOption { get }
```

## Discussion

List all windows, including both onscreen and offscreen windows. When retrieving a list with this option, the `relativeToWindow` parameter should be set to kCGNullWindowID.

## See Also

### Type Properties

static var excludeDesktopElements: CGWindowListOption

static var optionIncludingWindow: CGWindowListOption

static var optionOnScreenAboveWindow: CGWindowListOption

static var optionOnScreenBelowWindow: CGWindowListOption

static var optionOnScreenOnly: CGWindowListOption

