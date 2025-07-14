

- AppKit
- NSWindowDelegate
-  windowDidMiniaturize(\_:) 

Instance Method

# windowDidMiniaturize(\_:)

Tells the delegate that the window has been minimized.

macOS 10.10+

``` source
@MainActor
optional func windowDidMiniaturize(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didMiniaturizeNotification.

## Discussion

You can retrieve the `NSWindow` object in question by sending object to `notification`.

## See Also

### Minimizing Windows

func windowWillMiniaturize(Notification)

Tells the delegate that the window is about to be minimized.

func windowDidDeminiaturize(Notification)

Tells the delegate that the window has been deminimized.

