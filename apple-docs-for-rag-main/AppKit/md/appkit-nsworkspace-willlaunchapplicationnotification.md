

- AppKit
- NSWorkspace
-  willLaunchApplicationNotification 

Type Property

# willLaunchApplicationNotification

A notification that the workspace posts when the Finder is about to launch an app.

macOS

``` source
class let willLaunchApplicationNotification: NSNotification.Name
```

## Discussion

The notification object is the shared `NSWorkspace` instance. The `userInfo` dictionary contains the applicationUserInfoKey key with a corresponding instance of NSRunningApplication that represents the affected app.

The system doesn’t post this notification for background apps or for apps that have the `LSUIElement` key in their `Info.plist` file. If you want to know when all apps (including background apps) launch or terminate, use key-value observing to monitor the value that returns from the runningApplications method.

Important

To receive this notification, use notificationCenter to register for it. If you use a different notification center to register, you won’t receive the notification.

## See Also

### Responding to Environment Notifications

class let didLaunchApplicationNotification: NSNotification.Name

A notification that the workspace posts when a new app starts up.

class let didTerminateApplicationNotification: NSNotification.Name

A notification that the workspace posts when an app finishes executing.

class let sessionDidBecomeActiveNotification: NSNotification.Name

A notification that the workspace posts after a user session switches in.

class let sessionDidResignActiveNotification: NSNotification.Name

A notification that the workspace posts before a user session switches out.

class let didHideApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder hides an app.

class let didUnhideApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder unhides an app.

class let didActivateApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder is about to activate an app.

class let didDeactivateApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder deactivates an app.

class let didRenameVolumeNotification: NSNotification.Name

A notification that the workspace posts when a volume changes its name or mount path.

class let didMountNotification: NSNotification.Name

A notification that the workspace posts when a new device mounts.

class let willUnmountNotification: NSNotification.Name

A notification that the workspace posts when the Finder is about to unmount a device.

class let didUnmountNotification: NSNotification.Name

A notification that the workspace posts when the Finder unmounts a device.

class let didChangeFileLabelsNotification: NSNotification.Name

A notification that the workspace posts when the Finder file labels or colors change.

class let activeSpaceDidChangeNotification: NSNotification.Name

A notification that the workspace posts when a Spaces change occurs.

class let didWakeNotification: NSNotification.Name

A notification that the workspace posts when the device wakes from sleep.

