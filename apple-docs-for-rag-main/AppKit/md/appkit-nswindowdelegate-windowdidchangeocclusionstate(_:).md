

- AppKit
- NSWindowDelegate
-  windowDidChangeOcclusionState(\_:) 

Instance Method

# windowDidChangeOcclusionState(\_:)

Tells the delegate that the window changed its occlusion state.

macOS 10.9+

``` source
@MainActor
optional func windowDidChangeOcclusionState(_ notification: Notification)
```

## Parameters 

`notification`  

An didChangeOcclusionStateNotification notification.

