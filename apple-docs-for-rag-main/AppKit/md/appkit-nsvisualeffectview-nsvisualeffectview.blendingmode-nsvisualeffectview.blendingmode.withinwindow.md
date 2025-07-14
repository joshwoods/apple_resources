

- AppKit
- NSVisualEffectView
- NSVisualEffectView.BlendingMode
-  NSVisualEffectView.BlendingMode.withinWindow 

Case

# NSVisualEffectView.BlendingMode.withinWindow

A mode that blends and blurs the visual effect view with contents behind the view in the current window only.

macOS 10.10+

``` source
case withinWindow
```

## Discussion

Views using this blending mode must not overlap each other.

## See Also

### Blend Modes

case behindWindow

A mode that blends and blurs the visual effect view with the contents behind the window, such as the desktop or other windows.

