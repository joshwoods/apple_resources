

- AppKit
- NSApplicationDelegate
-  applicationShouldHandleReopen(\_:hasVisibleWindows:) 

Instance Method

# applicationShouldHandleReopen(\_:hasVisibleWindows:)

Returns a Boolean value that indicates if the app responds to reopen AppleEvents.

macOS

``` source
@MainActor
optional func applicationShouldHandleReopen(
    _ sender: NSApplication,
    hasVisibleWindows: Bool
) -> Bool
```

## Parameters 

`sender`  

The application object.

`hasVisibleWindows`  

Indicates whether the `NSApplication` object found any visible windows in your application. You can use this value as an indication of whether the application would do anything if you return true.

## Return Value

true if you want the application to perform its normal tasks or false if you want the application to do nothing.

## Discussion

These events are sent whenever the Finder reactivates an already running application because someone double-clicked it again or used the dock to activate it.

By default the Application Kit will handle this event by checking whether there are any visible `NSWindow` (not `NSPanel`) objects, and, if there are none, it goes through the standard untitled document creation (the same as it does if `theApplication` is launched without any document to open). For most document-based applications, an untitled document will be created.

The application delegate will also get a chance to respond to the normal untitled document delegate methods. If you implement this method in your application delegate, it will be called before any of the default behavior happens. If you return true, then `NSApplication` will proceed as normal. If you return false, then `NSApplication` will do nothing. So, you can either implement this method with a version that does nothing, and return false if you do not want anything to happen at all (not recommended), or you can implement this method, handle the event yourself in some custom way, and return false.

Miniaturized windows, windows in the Dock, are considered visible by this method, and cause `flag` to return true, despite the fact that miniaturized windows return false when sent an isVisible message.

## See Also

### Managing Windows

func applicationWillUpdate(Notification)

Tells the delegate that the app is about to update its windows.

func applicationDidUpdate(Notification)

Tells the delegate that the app’s windows did update.

