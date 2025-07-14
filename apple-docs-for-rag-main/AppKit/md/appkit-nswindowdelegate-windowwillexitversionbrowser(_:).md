

- AppKit
- NSWindowDelegate
-  windowWillExitVersionBrowser(\_:) 

Instance Method

# windowWillExitVersionBrowser(\_:)

Tells the delegate that the window is about to leave version browsing.

macOS 10.7+

``` source
@MainActor
optional func windowWillExitVersionBrowser(_ notification: Notification)
```

## Parameters 

`notification`  

An willExitVersionBrowserNotification notification.

## See Also

### Managing Presentation in Version Browsers

func window(NSWindow, willResizeForVersionBrowserWithMaxPreferredSize: NSSize, maxAllowedSize: NSSize) -> NSSize

Tells the delegate the window will resize for presentation during version browsing.

func windowWillEnterVersionBrowser(Notification)

Tells the delegate the window is about to enter version browsing.

func windowDidEnterVersionBrowser(Notification)

Tells the delegate that the window has entered version browsing.

func windowDidExitVersionBrowser(Notification)

Tells the delegate that the window has left version browsing.

