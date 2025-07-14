

- AppKit
- NSVisualEffectView
-  blendingMode 

Instance Property

# blendingMode

A value indicating how the view’s contents blend with the surrounding content.

macOS 10.10+

``` source
@MainActor
var blendingMode: NSVisualEffectView.BlendingMode { get set }
```

## Discussion

When the value of this property is NSVisualEffectView.BlendingMode.behindWindow (the default), the visual effect view blurs the content behind the window. When the value is NSVisualEffectView.BlendingMode.withinWindow, it blurs the content behind the view of the current window.

If the visual effect view’s material is NSVisualEffectView.Material.titlebar, set the blending mode to NSVisualEffectView.BlendingMode.withinWindow.

## See Also

### Specifying the Effect Appearance

enum BlendingMode

Constants that specify whether the visual effect view blends with what’s either behind or within the window.

var isEmphasized: Bool

A Boolean value indicating whether to emphasize the look of the material.

var interiorBackgroundStyle: NSView.BackgroundStyle

The view’s interior background style.

