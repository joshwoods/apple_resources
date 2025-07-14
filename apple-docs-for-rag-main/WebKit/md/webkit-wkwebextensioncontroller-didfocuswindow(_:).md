

- WebKit
- WKWebExtensionController
-  didFocusWindow(\_:) 

Instance Method

# didFocusWindow(\_:)

Should be called by the app when a window gains focus to fire appropriate events with all loaded web extensions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func didFocusWindow(_ focusedWindow: (any WKWebExtensionWindow)?)
```

## Parameters 

`focusedWindow`  

The window that gained focus, or \c nil if no window has focus or a window has focus that is not visible to extensions.

## Discussion

This method informs all loaded extensions of the focused window, ensuring consistent understanding across extensions.

If the intention is to inform only a specific extension, you should use the respective method on that extension’s context instead.

