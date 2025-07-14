

- AppKit
- NSWindowDelegate
-  windowDidDeminiaturize(\_:) 

Instance Method

# windowDidDeminiaturize(\_:)

Tells the delegate that the window has been deminimized.

macOS 10.10+

``` source
@MainActor
optional func windowDidDeminiaturize(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didDeminiaturizeNotification

## Discussion

You can retrieve the `NSWindow` object in question by sending object to `notification`.

## See Also

### Minimizing Windows

func windowWillMiniaturize(Notification)

Tells the delegate that the window is about to be minimized.

func windowDidMiniaturize(Notification)

Tells the delegate that the window has been minimized.

