

- AppKit
- NSWindowDelegate
-  windowWillMiniaturize(\_:) 

Instance Method

# windowWillMiniaturize(\_:)

Tells the delegate that the window is about to be minimized.

macOS 10.10+

``` source
@MainActor
optional func windowWillMiniaturize(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named willMiniaturizeNotification.

## Discussion

You can retrieve the `NSWindow` object in question by sending object to `notification`.

## See Also

### Minimizing Windows

func windowDidMiniaturize(Notification)

Tells the delegate that the window has been minimized.

func windowDidDeminiaturize(Notification)

Tells the delegate that the window has been deminimized.

