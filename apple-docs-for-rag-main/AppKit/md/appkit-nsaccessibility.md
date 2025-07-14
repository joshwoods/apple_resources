

- AppKit
-  NSAccessibility 

Structure

# NSAccessibility

A namespace for accessibility symbols for AppKit apps.

macOS

``` source
struct NSAccessibility
```

## Topics

### Posting Notifications

static func post(element: Any, notification: NSAccessibility.Notification)

Sends a notification to any observing assistive apps.

static func post(element: Any, notification: NSAccessibility.Notification, userInfo: [NSAccessibility.NotificationUserInfoKey : Any]?)

Sends a notification and an optional user info dictionary to any observing assistive apps.

### Getting Accessibility Objects

static func unignoredAncestor(of: Any) -> Any?

Returns an unignored accessibility object, ascending the hierarchy, if necessary.

static func unignoredChildren(from: [Any]) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredChildrenForOnlyChild(from: Any) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredDescendant(of: Any) -> Any?

Returns an unignored accessibility object, descending the hierarchy, if necessary.

### Getting Screen Coordinates

static func screenPoint(fromView: NSView, point: NSPoint) -> NSPoint

Returns the point in screen coordinates.

static func screenRect(fromView: NSView, rect: NSRect) -> NSRect

Returns the frame in screen coordinates.

### Specifying Protected Content

static func setMayContainProtectedContent(Bool) -> Bool

Sets whether the app may have protected content.

### Handling Errors

static let ErrorCodeExceptionInfo: String

An integer error code for debugging.

### Using Accessibility Types

struct Action

Constants that describe types of actions.

struct AnnotationAttributeKey

Keys for annotation attributes.

struct Attribute

Constants that describe attributes.

struct FontAttributeKey

Keys for font attributes.

struct Notification

The name of the notification.

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

### Deprecated

static func raiseBadArgumentException(Any!, NSAccessibility.Attribute!, Any!)

Raises an error if the parameter is the wrong type or has an illegal value

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### AppKit Elements

protocol NSAccessibilityProtocol

The complete list of properties and methods for accessible elements.

