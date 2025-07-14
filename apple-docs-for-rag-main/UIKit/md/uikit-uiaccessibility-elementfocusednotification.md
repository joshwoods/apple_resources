

- UIKit
- UIAccessibility
-  elementFocusedNotification 

Type Property

# elementFocusedNotification

A notification that UIKit posts when an assistive app focuses on an accessibility element.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
nonisolated
static let elementFocusedNotification: NSNotification.Name
```

## Discussion

Retrieve the focusedElementUserInfoKey key from the userInfo dictionary to get the identity of the focused accessibility element.

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

static let reduceTransparencyStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Reduce Transparency setting changes.

static let buttonShapesEnabledStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Button Shapes setting changes.

