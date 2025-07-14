

- AppKit
- NSVisualEffectView
- NSVisualEffectView.BlendingMode
-  NSVisualEffectView.BlendingMode.behindWindow 

Case

# NSVisualEffectView.BlendingMode.behindWindow

A mode that blends and blurs the visual effect view with the contents behind the window, such as the desktop or other windows.

macOS 10.10+

``` source
case behindWindow
```

## Discussion

Views using this blending mode can overlap, and the view lower in the hierarchy “wins”.

## See Also

### Blend Modes

case withinWindow

A mode that blends and blurs the visual effect view with contents behind the view in the current window only.

