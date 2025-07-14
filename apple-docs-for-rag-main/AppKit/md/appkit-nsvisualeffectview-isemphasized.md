

- AppKit
- NSVisualEffectView
-  isEmphasized 

Instance Property

# isEmphasized

A Boolean value indicating whether to emphasize the look of the material.

macOS 10.12+

``` source
@MainActor
var isEmphasized: Bool { get set }
```

## Discussion

Some materials change their appearance when they are emphasized. For example, the first responder view conveys its status.

The default value of this property is false.

## See Also

### Specifying the Effect Appearance

var blendingMode: NSVisualEffectView.BlendingMode

A value indicating how the view’s contents blend with the surrounding content.

enum BlendingMode

Constants that specify whether the visual effect view blends with what’s either behind or within the window.

var interiorBackgroundStyle: NSView.BackgroundStyle

The view’s interior background style.

