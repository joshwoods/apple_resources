

- Core Graphics
- CGWindowListOption
-  optionIncludingWindow 

Type Property

# optionIncludingWindow

Mac CatalystmacOS

``` source
static var optionIncludingWindow: CGWindowListOption { get }
```

## Discussion

Include the specified window (from the `relativeToWindow` parameter) in the returned list. You must combine this option with the optionOnScreenAboveWindow or optionOnScreenBelowWindow option to retrieve meaningful results.

## See Also

### Type Properties

static var excludeDesktopElements: CGWindowListOption

static var optionAll: CGWindowListOption

static var optionOnScreenAboveWindow: CGWindowListOption

static var optionOnScreenBelowWindow: CGWindowListOption

static var optionOnScreenOnly: CGWindowListOption

