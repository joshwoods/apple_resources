

- AppKit
- NSAccessibility
- NSAccessibility.Notification
-  windowResized 

Type Property

# windowResized

This notification is posted after a window’s size changes. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

macOS

``` source
static let windowResized: NSAccessibility.Notification
```

## See Also

### Notification Names

static let announcementRequested: NSAccessibility.Notification

This notification is posted whenever an accessibility element needs to make an announcement to the user. This notification requires a `userInfo` dictionary with the key announcement and a localized string containing the announcement. To help an assistive app determine the importance of the announcement, add the appropriate priority to the `userInfo` dictionary.

static let applicationActivated: NSAccessibility.Notification

This notification is posted after the app has been activated. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let applicationDeactivated: NSAccessibility.Notification

This notification is posted after the app has been deactivated. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let applicationHidden: NSAccessibility.Notification

This notification is posted after the app is hidden. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let applicationShown: NSAccessibility.Notification

This notification is posted after the app is shown. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let created: NSAccessibility.Notification

This notification is posted after an accessibility element is created. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let drawerCreated: NSAccessibility.Notification

This notification is posted after a drawer appears. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let focusedUIElementChanged: NSAccessibility.Notification

This notification is posted after an accessibility element gains focus. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let focusedWindowChanged: NSAccessibility.Notification

This notification is posted after the key window changes. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let helpTagCreated: NSAccessibility.Notification

This notification is posted after a help tag appears. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let layoutChanged: NSAccessibility.Notification

This notification is posted after the UI changes in a way that requires the attention of an accessibility client. This notification should be accompanied by a `userInfo` dictionary with the key uiElements and an array containing the UI elements that have been added or changed. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let mainWindowChanged: NSAccessibility.Notification

This notification is posted after the main window changes. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let moved: NSAccessibility.Notification

This notification is posted after an accessibility element moves. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let resized: NSAccessibility.Notification

This notification is posted after an accessibility element’s size changes. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let rowCollapsed: NSAccessibility.Notification

This notification is posted after a row collapses. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

