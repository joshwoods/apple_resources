

- UIKit
- UIAccessibility
-  reduceTransparencyStatusDidChangeNotification 

Type Property

# reduceTransparencyStatusDidChangeNotification

A notification that UIKit posts when the system’s Reduce Transparency setting changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let reduceTransparencyStatusDidChangeNotification: NSNotification.Name
```

## Discussion

This notification doesn’t include a parameter. Observe this notification using the default notification center.

## See Also

### UI changes

static let screenChanged: UIAccessibility.Notification

A notification that an app posts when a new view appears that occupies a major portion of the screen.

static let layoutChanged: UIAccessibility.Notification

A notification that an app posts when the layout of a screen changes.

static let pageScrolled: UIAccessibility.Notification

A notification that an app posts when a scroll action completes.

static let switchControlStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Switch Control setting changes.

static let elementFocusedNotification: NSNotification.Name

A notification that UIKit posts when an assistive app focuses on an accessibility element.

static let buttonShapesEnabledStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Button Shapes setting changes.

