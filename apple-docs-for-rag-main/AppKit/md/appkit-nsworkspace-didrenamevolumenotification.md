

- AppKit
- NSWorkspace
-  didRenameVolumeNotification 

Type Property

# didRenameVolumeNotification

A notification that the workspace posts when a volume changes its name or mount path.

macOS 10.6+

``` source
class let didRenameVolumeNotification: NSNotification.Name
```

## Discussion

These notifications typically change simultaneously, in which case, the workspace posts only one notification.

The notification object is the shared NSWorkspace instance. The `userInfo` dictionary may contain the following keys:

- localizedVolumeNameUserInfoKey

- volumeURLUserInfoKey

- oldLocalizedVolumeNameUserInfoKey

- oldVolumeURLUserInfoKey

Important

To receive this notification, use notificationCenter to register for it. If you use a different notification center to register, you won’t receive the notification.

## See Also

### Responding to Environment Notifications

class let willLaunchApplicationNotification: NSNotification.Name

A notification that the workspace posts when the Finder is about to launch an app.

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

