

- UIKit
- UIScreen
-  capturedDidChangeNotification 

Type Property

# capturedDidChangeNotification

A notification that posts when the capture status of a screen changes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+

``` source
nonisolated
class let capturedDidChangeNotification: NSNotification.Name
```

## Discussion

The contents of a screen can be recorded, mirrored, sent over AirPlay, or otherwise cloned to another destination. UIKit sends this notification when the capture status of the screen changes.

The object of the notification is the UIScreen object whose isCaptured property changed. There is no `userInfo` dictionary.

The system posts this notification on the main actor.

## See Also

### Notifications

class let brightnessDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s brightness changes.

class let modeDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s mode changes.

class let referenceDisplayModeStatusDidChangeNotification: NSNotification.Name

A notification that posts when there’s a change to a screen’s reference display mode status.

