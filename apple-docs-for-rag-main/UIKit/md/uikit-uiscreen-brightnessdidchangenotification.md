

- UIKit
- UIScreen
-  brightnessDidChangeNotification 

Type Property

# brightnessDidChangeNotification

A notification that posts when a screen’s brightness changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOS

``` source
nonisolated
class let brightnessDidChangeNotification: NSNotification.Name
```

## Discussion

The object of the notification is the UIScreen object whose brightness property changed. There is no `userInfo` dictionary.

## See Also

### Notifications

class let modeDidChangeNotification: NSNotification.Name

A notification that posts when a screen’s mode changes.

class let capturedDidChangeNotification: NSNotification.Name

A notification that posts when the capture status of a screen changes.

class let referenceDisplayModeStatusDidChangeNotification: NSNotification.Name

A notification that posts when there’s a change to a screen’s reference display mode status.

