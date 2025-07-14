

- UIKit
- UIWindowScene
-  keyWindow 

Instance Property

# keyWindow

The key window associated with the scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var keyWindow: UIWindow? { get }
```

## Discussion

The key window receives keyboard and other non-touch-related events. Of a scene’s associated windows, only one window at a time may be the key window.

## See Also

### Getting the active windows

var windows: [UIWindow]

The windows associated with the scene.

var screen: UIScreen

The screen that displays the contents of the scene.

