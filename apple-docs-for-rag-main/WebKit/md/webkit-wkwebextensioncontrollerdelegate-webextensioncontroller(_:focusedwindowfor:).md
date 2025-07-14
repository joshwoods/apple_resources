

- WebKit
- WKWebExtensionControllerDelegate
-  webExtensionController(\_:focusedWindowFor:) 

Instance Method

# webExtensionController(\_:focusedWindowFor:)

Called when an extension context requests the currently focused window.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func webExtensionController(
    _ controller: WKWebExtensionController,
    focusedWindowFor extensionContext: WKWebExtensionContext
) -> (any WKWebExtensionWindow)?
```

## Parameters 

`controller`  

The web extension controller that is managing the extension.

`extensionContext`  

The context in which the web extension is running.

## Discussion

This method can be optionally implemented by the app to designate the window currently in focus to the extension.

If not implemented, the first window in the result of webExtensionController(_:openWindowsFor:) is used.

## See Also

### Related Documentation

func webExtensionController(WKWebExtensionController, openWindowsFor: WKWebExtensionContext) -> [any WKWebExtensionWindow]

Called when an extension context requests the list of ordered open windows.

