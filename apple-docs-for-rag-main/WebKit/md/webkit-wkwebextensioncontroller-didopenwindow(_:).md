

- WebKit
- WKWebExtensionController
-  didOpenWindow(\_:) 

Instance Method

# didOpenWindow(\_:)

Should be called by the app when a new window is opened to fire appropriate events with all loaded web extensions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func didOpenWindow(_ newWindow: any WKWebExtensionWindow)
```

## Parameters 

`newWindow`  

The newly opened window.

## Discussion

This method informs all loaded extensions of the opening of a new window, ensuring consistent understanding across extensions.

If the intention is to inform only a specific extension, you should use the respective method on that extension’s context instead.

## See Also

### Related Documentation

func didCloseWindow(any WKWebExtensionWindow)

Should be called by the app when a window is closed to fire appropriate events with all loaded web extensions.

