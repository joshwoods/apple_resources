

- AppKit
- NSColorWell
-  supportsAlpha 

Instance Property

# supportsAlpha

A Boolean value that determines whether the color picker supports alpha values.

macOS 14.0+

``` source
@MainActor
var supportsAlpha: Bool { get set }
```

## Discussion

If this property is false, people can select only fully opaque colors from the color picker. A value of false also hides the alpha slider. Setting this property to true enables partial color opacity, and also makes the alpha slider visible.

If ignoresAlpha is true, this property always returns false, disabling alpha globally.

By default this value is true.

## See Also

### Managing the Selected Color

var color: NSColor

The currently selected color for the color well.

func takeColorFrom(Any?)

Changes the currently selected color to the color of the specified object.

