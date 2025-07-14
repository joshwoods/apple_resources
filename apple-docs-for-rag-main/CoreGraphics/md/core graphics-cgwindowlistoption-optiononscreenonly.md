

- Core Graphics
- CGWindowListOption
-  optionOnScreenOnly 

Type Property

# optionOnScreenOnly

Mac CatalystmacOS

``` source
static var optionOnScreenOnly: CGWindowListOption { get }
```

## Discussion

List all windows that are currently onscreen. Windows are returned in order from front to back. When retrieving a list with this option, the `relativeToWindow` parameter should be set to kCGNullWindowID.

## See Also

### Type Properties

static var excludeDesktopElements: CGWindowListOption

static var optionAll: CGWindowListOption

static var optionIncludingWindow: CGWindowListOption

static var optionOnScreenAboveWindow: CGWindowListOption

static var optionOnScreenBelowWindow: CGWindowListOption

