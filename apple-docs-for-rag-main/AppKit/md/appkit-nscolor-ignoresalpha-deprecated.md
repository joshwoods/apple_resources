

- AppKit
- NSColor
-  ignoresAlpha Deprecated

Type Property

# ignoresAlpha

A Boolean value that indicates whether the app supports alpha.

macOS 10.0–14.0Deprecated

``` source
@MainActor
class var ignoresAlpha: Bool { get set }
```

Deprecated

Use showsAlpha and supportsAlpha to manage alpha behavior for individual controls.

## Return Value

true if the app doesn’t support alpha; otherwise, false.

## Discussion

The system consults this global value when the app imports alpha (for instance, through color dragging). By default this property is false; meaning the system supports the alpha component for colors globally. To ignore alpha for an app, invoke the `setIgnoresAlpha` method with a parameter of true. This value also determines whether the color panel has an opacity slider.

This method provides a global approach for removing alpha, which might not always be appropriate. Apps that need to disable alpha can use more fine-grained APIs for individual controls, such as showsAlpha and supportsAlpha.

In macOS 13 and earlier, the default value is true. This property is deprecated as of macOS 14.

## See Also

### Related Documentation

var alphaComponent: CGFloat

The alpha (opacity) component value of the color.

