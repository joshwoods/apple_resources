

- AppKit
- NSVisualEffectView
-  interiorBackgroundStyle 

Instance Property

# interiorBackgroundStyle

The view’s interior background style.

macOS 10.10+

``` source
@MainActor
var interiorBackgroundStyle: NSView.BackgroundStyle { get }
```

## Discussion

The background style may be light or dark, depending on the selected material.

## See Also

### Specifying the Effect Appearance

var blendingMode: NSVisualEffectView.BlendingMode

A value indicating how the view’s contents blend with the surrounding content.

enum BlendingMode

Constants that specify whether the visual effect view blends with what’s either behind or within the window.

var isEmphasized: Bool

A Boolean value indicating whether to emphasize the look of the material.

