

- ScreenCaptureKit
- SCWindow
-  isActive 

Instance Property

# isActive

A Boolean value that indicates if the window is currently streaming.

Mac Catalyst 16.2+macOS 13.1+

``` source
var isActive: Bool { get }
```

## Discussion

When this value is `true`, the window is currently streaming, even if offscreen.

## See Also

### Determining visibility

var isOnScreen: Bool

A Boolean value that indicates whether the window is on screen.

