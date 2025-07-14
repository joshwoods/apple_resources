

- UIKit
- UIScreen
-  modeDidChangeNotification 

Type Property

# modeDidChangeNotification

A notification that posts when a screen’s mode changes.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOS

``` source
nonisolated
class let modeDidChangeNotification: NSNotification.Name
```

## Mentioned in 

Processing queued notifications

## Discussion

Clients can use this notification to detect changes in the screen resolution.

The object of the notification is the UIScreen object whose currentMode property changed. There is no `userInfo` dictionary.

The system posts this notification on the main actor.

## See Also

### Notifications

class let brightnessDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s brightness changes.

class let capturedDidChangeNotification: NSNotification.Name

A notification that posts when the capture status of a screen changes.

class let referenceDisplayModeStatusDidChangeNotification: NSNotification.Name

A notification that posts when there’s a change to a screen’s reference display mode status.

