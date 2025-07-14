

- AppKit
- NSAccessibility
-  NSAccessibility.Notification 

Structure

# NSAccessibility.Notification

The name of the notification.

macOS

``` source
struct Notification
```

## Topics

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

static let rowCountChanged: NSAccessibility.Notification

This notification is posted after a row is added or deleted. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let rowExpanded: NSAccessibility.Notification

This notification is posted after a row expands. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let selectedCellsChanged: NSAccessibility.Notification

This notification is posted after one or more cells in a cell-based table are selected or deselected. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let selectedChildrenChanged: NSAccessibility.Notification

This notification is posted after one or more child elements are selected or deselected. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let selectedChildrenMoved: NSAccessibility.Notification

This notification is posted after the selected items in a layout area move. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let selectedColumnsChanged: NSAccessibility.Notification

This notification is posted after one or more columns are selected or deselected. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let selectedRowsChanged: NSAccessibility.Notification

This notification is posted after one or more rows are selected or deselected. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let selectedTextChanged: NSAccessibility.Notification

This notification is posted after text is selected or deselected. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let sheetCreated: NSAccessibility.Notification

This notification is posted after a sheet appears. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let titleChanged: NSAccessibility.Notification

This notification is posted after an accessibility element’s title changes. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let uiElementDestroyed: NSAccessibility.Notification

This notification is posted after an accessibility element is destroyed. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let unitsChanged: NSAccessibility.Notification

This notification is posted after the units in a layout area change. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let valueChanged: NSAccessibility.Notification

This notification is posted after an accessibility element’s value changes. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let windowCreated: NSAccessibility.Notification

This notification is posted after a new window appears. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let windowDeminiaturized: NSAccessibility.Notification

This notification is posted after a window is restored to full size from the Dock. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let windowMiniaturized: NSAccessibility.Notification

This notification is posted after a window is put in the Dock. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let windowMoved: NSAccessibility.Notification

This notification is posted after a window moves. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

static let windowResized: NSAccessibility.Notification

This notification is posted after a window’s size changes. Post this notification using the post(element:notification:) function instead of an `NSNotificationCenter` instance.

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Using Accessibility Types

struct Action

Constants that describe types of actions.

struct AnnotationAttributeKey

Keys for annotation attributes.

struct Attribute

Constants that describe attributes.

struct FontAttributeKey

Keys for font attributes.

struct NotificationUserInfoKey

The key in the user info dictionary for a notification.

struct OrientationValue

Values that indicate the orientation of user interface elements, such as scroll bars and split views.

struct ParameterizedAttribute

Values that describe parameterized attributes.

struct Role

Values that describe types of objects that accessibility elements represent.

struct RulerMarkerTypeValue

Values that describe ruler marker types.

struct RulerUnitValue

Values that indicate the unit values of a ruler or layout area.

struct SortDirectionValue

Values that indicate the sort direction of a column.

struct Subrole

Values that describe specialized object subtypes that accessibility elements represent.

