

- AppKit
- NSApplication
-  willHideNotification 

Type Property

# willHideNotification

Posted at the start of the hide(_:) method to indicate that the app is about to be hidden.

macOS

``` source
class let willHideNotification: NSNotification.Name
```

## Discussion

The notification object is `NSApp`. This notification doesn’t contain a `userInfo` dictionary.

## See Also

### Notifications

class let didBecomeActiveNotification: NSNotification.Name

Posted immediately after the app becomes active.

class let didChangeScreenParametersNotification: NSNotification.Name

Posted when the configuration of the displays attached to the computer is changed.

class let didFinishLaunchingNotification: NSNotification.Name

Posted at the end of the finishLaunching() method to indicate that the app has completed launching and is ready to run.

class let didHideNotification: NSNotification.Name

Posted at the end of the hide(_:) method to indicate that the app is now hidden.

class let didResignActiveNotification: NSNotification.Name

Posted immediately after the app gives up its active status to another app.

class let didUnhideNotification: NSNotification.Name

Posted at the end of the unhideWithoutActivation() method to indicate that the app is now visible.

class let didUpdateNotification: NSNotification.Name

Posted at the end of the updateWindows() method to indicate that the app has finished updating its windows.

class let willBecomeActiveNotification: NSNotification.Name

Posted immediately before the app becomes active.

class let willFinishLaunchingNotification: NSNotification.Name

Posted at the start of the finishLaunching() method to indicate that the app has completed its initialization process and is about to finish launching.

class let willResignActiveNotification: NSNotification.Name

Posted immediately before the app gives up its active status to another app.

class let willTerminateNotification: NSNotification.Name

Sends a notification to termintate the app.

class let willUnhideNotification: NSNotification.Name

Posted at the start of the unhideWithoutActivation() method to indicate that the app is about to become visible.

class let willUpdateNotification: NSNotification.Name

Posted at the start of the updateWindows() method to indicate that the app is about to update its windows.

class let didFinishRestoringWindowsNotification: NSNotification.Name

Posted when the app has finished restoring windows.

class let didChangeOcclusionStateNotification: NSNotification.Name

Posted when the app’s occlusion state changes.

