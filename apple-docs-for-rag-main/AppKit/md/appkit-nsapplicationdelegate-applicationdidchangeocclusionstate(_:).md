

- AppKit
- NSApplicationDelegate
-  applicationDidChangeOcclusionState(\_:) 

Instance Method

# applicationDidChangeOcclusionState(\_:)

Tells the delegate about changes to the app’s occlusion state.

macOS 10.9+

``` source
@MainActor
optional func applicationDidChangeOcclusionState(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named didChangeOcclusionStateNotification. Calling the object method of this notification returns the `NSApplication` object itself.

## Discussion

Upon receiving this method, you can query the application for its occlusion state. Note that this only notifies about changes in the state of the occlusion, not when the occlusion region changes. You can use this method to increase responsiveness and save power by halting any expensive calculations that the user can not see.

