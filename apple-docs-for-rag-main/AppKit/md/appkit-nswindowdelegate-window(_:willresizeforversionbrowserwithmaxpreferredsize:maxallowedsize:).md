

- AppKit
- NSWindowDelegate
-  window(\_:willResizeForVersionBrowserWithMaxPreferredSize:maxAllowedSize:) 

Instance Method

# window(\_:willResizeForVersionBrowserWithMaxPreferredSize:maxAllowedSize:)

Tells the delegate the window will resize for presentation during version browsing.

macOS 10.7+

``` source
@MainActor
optional func window(
    _ window: NSWindow,
    willResizeForVersionBrowserWithMaxPreferredSize maxPreferredFrameSize: NSSize,
    maxAllowedSize maxAllowedFrameSize: NSSize
) -> NSSize
```

## Parameters 

`window`  

The window being presented in a version browser.

`maxPreferredFrameSize`  

The maximum size the version browser would prefer the window to be.

`maxAllowedFrameSize`  

The maximum allowed size for the window (the full-screen frame minus the margins required to ensure the Versions controls are still visible).

## Return Value

The size that the window should be.

## Discussion

Windows entering the version browser will be resized to the size returned by this method. If either dimension of the returned size is larger than the `maxPreferredFrameSize`, the window will also be scaled down to ensure it fits properly in the version browser.

If this method is not implemented, the version browser will use windowWillUseStandardFrame(_:defaultFrame:) to determine the resulting window frame size.

## See Also

### Managing Presentation in Version Browsers

func windowWillEnterVersionBrowser(Notification)

Tells the delegate the window is about to enter version browsing.

func windowDidEnterVersionBrowser(Notification)

Tells the delegate that the window has entered version browsing.

func windowWillExitVersionBrowser(Notification)

Tells the delegate that the window is about to leave version browsing.

func windowDidExitVersionBrowser(Notification)

Tells the delegate that the window has left version browsing.

