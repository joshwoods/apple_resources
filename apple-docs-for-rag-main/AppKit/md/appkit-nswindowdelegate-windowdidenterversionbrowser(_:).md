

- AppKit
- NSWindowDelegate
-  windowDidEnterVersionBrowser(\_:) 

Instance Method

# windowDidEnterVersionBrowser(\_:)

Tells the delegate that the window has entered version browsing.

macOS 10.7+

``` source
@MainActor
optional func windowDidEnterVersionBrowser(_ notification: Notification)
```

## Parameters 

`notification`  

An didEnterVersionBrowserNotification notification.

## See Also

### Managing Presentation in Version Browsers

func window(NSWindow, willResizeForVersionBrowserWithMaxPreferredSize: NSSize, maxAllowedSize: NSSize) -> NSSize

Tells the delegate the window will resize for presentation during version browsing.

func windowWillEnterVersionBrowser(Notification)

Tells the delegate the window is about to enter version browsing.

func windowWillExitVersionBrowser(Notification)

Tells the delegate that the window is about to leave version browsing.

func windowDidExitVersionBrowser(Notification)

Tells the delegate that the window has left version browsing.

