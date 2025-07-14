

- UIKit
- UIAccessibility
- UIAccessibility.Notification
-  layoutChanged 

Type Property

# layoutChanged

A notification that an app posts when the layout of a screen changes.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
nonisolated
static let layoutChanged: UIAccessibility.Notification
```

## Discussion

Post this notification using the post(notification:argument:) function. Optionally, include a parameter that contains the accessibility element for VoiceOver to move to after processing the notification.

## See Also

### UI changes

static let screenChanged: UIAccessibility.Notification

A notification that an app posts when a new view appears that occupies a major portion of the screen.

static let pageScrolled: UIAccessibility.Notification

A notification that an app posts when a scroll action completes.

static let switchControlStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Switch Control setting changes.

static let elementFocusedNotification: NSNotification.Name

A notification that UIKit posts when an assistive app focuses on an accessibility element.

static let reduceTransparencyStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Reduce Transparency setting changes.

static let buttonShapesEnabledStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Button Shapes setting changes.

