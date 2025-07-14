

- UIKit
- UIScreen
-  referenceDisplayModeStatusDidChangeNotification 

Type Property

# referenceDisplayModeStatusDidChangeNotification

A notification that posts when there’s a change to a screen’s reference display mode status.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+

``` source
nonisolated
class let referenceDisplayModeStatusDidChangeNotification: NSNotification.Name
```

## Discussion

The notification’s object is the changed screen. Use that object’s referenceDisplayModeStatus property to retrieve the new status.

The system posts this notification on the main actor.

## See Also

### Notifications

class let brightnessDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s brightness changes.

class let modeDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s mode changes.

class let capturedDidChangeNotification: NSNotification.Name

A notification that posts when the capture status of a screen changes.

