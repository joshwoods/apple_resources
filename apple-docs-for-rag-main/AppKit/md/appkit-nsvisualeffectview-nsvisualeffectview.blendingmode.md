

- AppKit
- NSVisualEffectView
-  NSVisualEffectView.BlendingMode 

Enumeration

# NSVisualEffectView.BlendingMode

Constants that specify whether the visual effect view blends with what’s either behind or within the window.

macOS 10.10+

``` source
enum BlendingMode
```

## Topics

### Blend Modes

case behindWindow

A mode that blends and blurs the visual effect view with the contents behind the window, such as the desktop or other windows.

case withinWindow

A mode that blends and blurs the visual effect view with contents behind the view in the current window only.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the Effect Appearance

var blendingMode: NSVisualEffectView.BlendingMode

A value indicating how the view’s contents blend with the surrounding content.

var isEmphasized: Bool

A Boolean value indicating whether to emphasize the look of the material.

var interiorBackgroundStyle: NSView.BackgroundStyle

The view’s interior background style.

