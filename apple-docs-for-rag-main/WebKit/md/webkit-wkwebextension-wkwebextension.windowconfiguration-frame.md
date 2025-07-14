

- WebKit
- WKWebExtension
- WKWebExtension.WindowConfiguration
-  frame 

Instance Property

# frame

Indicates the frame where the window should be positioned on the main screen.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var frame: CGRect { get }
```

## Discussion

This frame should override the app’s default window position and size.

Individual components (e.g., `origin.x`, `size.width`) will be `NaN` if not specified.

